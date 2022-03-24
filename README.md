# Fenics-Tensile

This WaNo uses the Finite Element Fenics library to compute the tensile properties of a cylindric body.

# Python dependencies

```
- python==3.9
- fenics==2019.1.0
- mshr==2019.1.0
- pyymal
```

# Create a conda environment:
```
conda create -n fenicsproject python=3.9 numpy fenics==2019.1.0 mshr==2019.1.0 pyyaml
```

Alternatively, you can run the script locally by executing the command below in the same folder where you saved the input (input.json). 

```
python tensile.py
```

# Usage in SimStack

For this particular WaNo, as shown in the figure below, you can run it in the mode, where you insert the parameter manually or by loading the inputs from a given '.json' file.

<img src="fenics_tensile.png" alt="drawing" width="300"/>

**Fig 1** The DFT-VASP WaNo performs DFT calculation using Vasp code. In this WaNo, the POTCAR might be automatized after reading the POSCAR file. In the GUI, we can set the KPOINTS and INCAR files, but there is also the option to load the inputs file in the Files_Run tab.

