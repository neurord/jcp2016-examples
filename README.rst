Example models for JCP 2016 article
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Asynchronous τ-leaping**,
Zbigniew Jędrzejewski-Szmek, Kim T. Blackwell,
Journal of Chemical Physics, **144**, 125104 (2016)

To run the examples:

1. clone this repository:

   .. code:: shell

     git clone https://github.com/neurord/jcp2016-examples

2. download NeuroRD v. 3.0:

   .. code:: shell

     wget https://github.com/neurord/stochdiff/releases/download/v3.0/stochdiff-3.0.0-all-deps.jar

3. pick one of the examples, e.g.:

   .. code:: shell

     cd jcp2016-examples/a_b_2d_c_annihilation/

4. run the simulation:

   .. code:: shell

     java -Dstochdiff.writers=h5,text -jar ../../stochdiff-3.0.0-all-deps.jar model-async-0.01.xml

This produces output of

* `*.h5` — the HDF5 file with simulation results (numbers of particles as specified times)
* `*.out` — the same but in tabular text format
* `*.log` — a copy of the screen output

See https://github.com/neurord/stochdiff/blob/v3.0/README.rst for documentation about
the model file format and runtime options.
