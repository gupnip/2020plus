Usage
-----

This project has only been tested on python 2.7.5

The requirements.txt file lists the python dependencies I used for developing
the package.

run.py is the single command line interface for this project.
Type python run.py --help for details.

NOTE: Run run.py while in the same directory. Because of package imports,
running from a different directory may cause an import error.

The matplotlibrc file is the configuration for plotting styles. If you prefer
a different plot style then just replace the config file from the styles directory.

Directories
-----------

* data_analysis -- outputs descriptive plots and results from COSMIC database
* data -- input data to program that is not from the COSMIC MySQL database
* classify -- analyzes results of classifying genes as oncogenes or tsg
* features -- generates/contains the features text file used for classification
* log -- contain log files from running run.py
* utils -- useful miscellaneous code for this package
* config -- contains configuration files for running code
* styles -- matplotlib styles for plotting
* tests -- unit tests to be tested by the python "nose" package
* results -- contains output from commands
* simulation -- simulate COSMIC database size changes