A model of production of cAMP stimulated by dopamine
====================================================

The morphology consists of three compartments: 1×1×0.25 µm²,
1×1×1 µm², 1×1×0.25 µm².

Species Da, ATP, cAMP, AMP, PKAc are diffusible. Other species
do not diffuse.

Reactions:

.. figure:: Rxn_cAMPassayPDE2.png
   :figwidth: 50%

* Da + D1R ↔ DaD1R
* DaD1R + Gsabg ↔ DaD1RGs
* Gsabg + D1R ↔ GsD1R
* GsD1R + Da ↔ DaD1RGs
* DaD1RGs → GasGTP
* DaD1RGbg → DaD1R + Gbg
* GasGTP → GasGDP
* GasGDP + Gbg → Gsabg
* GasGTP + AC ↔ ACGas
* ACGas + ATP ↔ ACGasATP
* ACGasATP ↔ ACGas + cAMP
* PDE10 + cAMP ↔ PDE10cAMP
* PDE10cAMP → PDE10 + AMP
* PKAc + PDE10 ↔ PKAcPDE10
* PKAcPDE10 → pPDE10 + PKAc
* PKAc + PDE10cAMP ↔ PKAcPDE10cAMP
* PKAcPDE10cAMP → pPDE10cAMP + PKAc
* pPDE10 → PDE10
* pPDE10 + cAMP ↔ pPDE10cAMP
* pPDE10cAMP → pPDE10 + AMP
* AMP → ATP
* PKA + 2cAMP ↔ PKAcAMP2
* PKAcAMP2 + 2cAMP ↔ PKAcAMP4
* PKAcAMP4 ↔ PKAr + 2PKAc
* PDE2 + cAMP ↔ PDE2cAMP
* PDE2cAMP + cAMP ↔ PDE2cAMP2
* PDE2cAMP2 → PDE2cAMP + AMP

See `reactions.xml` for reaction and diffusion constants.

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

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_ATP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_Da.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_PDE2cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_PKAcAMP2.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_PKAcPDE10.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_PKAc.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_pPDE10cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.001,_particle_numbers_of_species_pPDE10.png
   :scale: 15%

Asynchronous leaping with ε=0.01
````````````````````````````````

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_ATP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_Da.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_PDE2cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_PKAcAMP2.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_PKAcPDE10.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_PKAc.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_pPDE10cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.01,_particle_numbers_of_species_pPDE10.png
   :scale: 15%

Asynchronous leaping with ε=0.1
```````````````````````````````

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_ATP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_Da.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_PDE2cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_PKAcAMP2.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_PKAcPDE10.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_PKAc.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_pPDE10cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-async-0.1,_particle_numbers_of_species_pPDE10.png
   :scale: 15%

Exact stochastic simulation
```````````````````````````

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_ATP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_Da.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_PDE2cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_PKAcAMP2.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_PKAcPDE10.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_PKAc.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_pPDE10cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-exact,_particle_numbers_of_species_pPDE10.png
   :scale: 15%

Fixed leaping with τ=0.005 ms
`````````````````````````````

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_ATP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_Da.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_PDE2cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_PKAcAMP2.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_PKAcPDE10.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_PKAc.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_pPDE10cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.005,_particle_numbers_of_species_pPDE10.png
   :scale: 15%

Fixed leaping with τ=0.05 ms
````````````````````````````

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_ATP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_Da.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_PDE2cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_PKAcAMP2.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_PKAcPDE10.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_PKAc.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_pPDE10cAMP.png
   :scale: 15%

.. figure:: Model_cAMPassay1.5-PDE2600-fixed-0.05,_particle_numbers_of_species_pPDE10.png
   :scale: 15%
