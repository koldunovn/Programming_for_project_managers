# Programming for project managers
[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/koldunovn/Programming_for_project_managers/master)

This repository contains supporting material for ADGEO paper "Programming as a soft skill for project managers: How to have a computer take over some of your work".

The easiest way to begin to work is to press "launch binder" button above. The environment with a running python kernel and all nessesary libraries will be launched, and you can begin interactive work with Jupyter notebooks in the repository straight away.

* [The introduction to the Jupyter Notebooks](https://www.youtube.com/watch?v=HW29067qVWk).

* [More in depth totorial](https://www.youtube.com/watch?v=VQBZ2MqWBZI).

## Local installation

In order to work with the Notebooks from this repository locally you have to have a python 3.6 installation as well as several additional packages. The easiest way to install them is to use `Miniconda`. Below you can find instructions for Linus/Mac and Windows.

### Installation for Linux/Mac

The fastest way is to install [Miniconda](http://conda.pydata.org/miniconda.html), that contains [`conda`](http://conda.pydata.org/docs/intro.html) package manager and `Python`. On the [Miniconda](http://conda.pydata.org/miniconda.html) page select **Python 3** installer script for your system and download it, for example:

```
wget https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
```

Change mode of the downloaded scrip to executable, e.g.:

```
chmod +x Miniconda3-latest-MacOSX-x86_64.sh
```

Run installation process:
```
./Miniconda3-latest-MacOSX-x86_64.sh
```
At the end the script will offer you to add Miniconda3 install location to the PATH in your `.bashrc/.bash_profile`. You should say 'yes'. Please double check that you have something like this in your `.bashrc/.bash_profile`:

```
# added by Miniconda3 4.3.21 installer
export PATH="/Users/koldunovn/miniconda3/bin:$PATH"
```
If you for whatever strange reason use csh/tcsh, then add to your `.cshrc`:

```
setenv PATH /Users/koldunovn/miniconda3/bin:$PATH
```
Now you can open a new terminal window (sourcing not always works) and try to type:

```
conda
```
if as a result you see conda help, then everything is set up properly. The last thing before installing packages is to add `conda-forge` channel:
```
conda config --add channels conda-forge 
```
Now you can install nessesary packages by executing this three lines:
```
conda install pandas=0.20.3, numpy=1.12.1 matplotlib=2.0.2 seaborn=0.8.1 pip
pip install python-docx==0.8.6
pip install openpyxl==2.5.1
```
To begin working with notebooks execute:
```
jupyter notebook
```
the browser should pop up with jupyter main page. You can navigate to the folder with notebooks from there and open them.

### Installation for Windows

- First you have to download and install Anaconda python distribution for your system from [here](http://continuum.io/downloads). If installation is sucessful, you will be able to work with notebooks from 02 to 07. In order to work with `netCDF` files and `Basemap` some additional steps are required.

- Go to start menu, choose `run` and execute `cmd` in order to bring up windows command line.
- Change to `Anaconda\Scripts` directory by executing `cd Anaconda\Scripts`
- execute `conda install pandas=0.20.3, numpy=1.12.1 matplotlib=2.0.2 seaborn=0.8.1 pip` and agree with installation
- execute `pip install python-docx==0.8.6` and agree with installation
- execute `pip install openpyxl==2.5.1` and agree with installation

### Download and run the code

You can download the code by pressing friendly green button at the upper right part of the repository with "clone or download" and select "download ZIP". Unpack the downloaded ZIP file and enter the resulting directory in your terminal. Type:

```
jupyter notebook
```

After some time your browser should start and show the list of the Notebook files (.ipynb) from the repository. If it doesn't, just copy the link that will apear in your terminal to the browser agress box. 

Authors
========
Nikolay Koldunov, Luisa Cristini

koldunovn@gmail.com
