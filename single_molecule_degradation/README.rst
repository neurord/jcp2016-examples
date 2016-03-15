First order degradation reaction
================================

A very simple model with the following reaction:

* A → Φ

See `reactions.xml` for reaction constants.

There are several model files in the directory, but all model files
are the same except for the specification of the method (at the end of
the file). Parameter ``<calculation>`` is ``GRID_EXACT`` for exact,
``GRID_STEPPED_STOCHASTIC`` for fixed-τ, and ``GRID_ADAPTIVE`` for
asynchronous. Both fixed-τ and asynchronous have one additional
parameter.  ``<tolerance>`` which is the accuracy control parameter
used for asynchronous and ``<fixedStepDt>`` which is the time step in
fixed-τ leaping.

Asynchronous leaping with ε=0.001
`````````````````````````````````

.. figure:: model-async-0.001,_particle_numbers_of_species_A.png

Asynchronous leaping with ε=0.01
````````````````````````````````

.. figure:: model-async-0.01,_particle_numbers_of_species_A.png

Asynchronous leaping with ε=0.1
```````````````````````````````

.. figure:: model-async-0.1,_particle_numbers_of_species_A.png

Exact stochastic simulation
```````````````````````````

.. figure:: model-exact,_particle_numbers_of_species_A.png

Fixed leaping with τ=0.5 ms   
```````````````````````````

.. figure:: model-step-0.5,_particle_numbers_of_species_A.png

Fixed leaping with τ=50 ms   
```````````````````````````

.. figure:: model-step-50.0,_particle_numbers_of_species_A.png
