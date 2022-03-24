# Fenics-Tensile
This WaNo uses the Finite Element Fenics library to compute the tensile properties of a cylindric body.

This is an example project on howto include script jobs in pyiron.

# Installation:
create a conda environment either locally (as shown here) using 
```
conda env create -f --prefix ./conda-env environment.yml
```
Alternative, you could also use the script 
```
make_environment.sh 
```
that either creates a new local environment or updates the existing one. 

Afterwards, activate the conda environment
```
conda activate ./conda-env 
```
and execute the script that creates a "~.pyiron" config file with the 
information where the scripts for the new script jobs are located.
```
python pyiron/pyiron_config.py
```

# Usage
script jobs have to be added to the resources/templates directory. Just add 
a new directory (the name is then automtically the jobname in pyiron) and 
add an input.json and a script.py in the newly created directory. 

The script.py should include your job definition, whereas the input.json 
defines standard parameters that can be changed.
