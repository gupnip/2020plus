Installation
------------

.. image:: https://travis-ci.org/KarchinLab/2020plus.svg?branch=master
    :target: https://travis-ci.org/KarchinLab/2020plus

Releases
~~~~~~~~

20/20+ can be downloaded on `github <https://github.com/KarchinLab/2020plus/releases>`_.
Once downloaded, either add the directory to your :code:`PATH` variable or issue the full path to the 2020plus.py script.

Package requirements
~~~~~~~~~~~~~~~~~~~~

Because 20/20+ internally uses the random forest package in R, you will both need `R <https://www.r-project.org/>`_ and the randomForest library installed. Once R is installed, you can install the random forest package:

.. code-block:: R

    > install.packages("randomForest")

If you do not have permission to install `randomForest` on the system wide R, you can install in your local user directory by creating an `~/.Renviron` file as the following:

.. code-block:: bash

    R_LIBS=~/Rlibs

Where, in this case, the R libraries will be installed in the `~/Rlibs` directory.

20/20+ also requires the following python packages:

* numpy
* scipy
* pandas>=0.17
* scikit-learn
* rpy2
* probabilistic2020

To install these packages via `pip` you can use the following command:

.. code-block:: bash

    $ pip install -r requirements.txt

If you want the exact version 20/20+ was tested on use the requirements_dev.txt file and python 2.7. The `probabilistic2020 <https://github.com/KarchinLab/probabilistic2020>`_ python package is used to generate features used by 20/20+ from the mutations in MAF format.
