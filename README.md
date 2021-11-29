# Jupyter Instructions

## **Prerequisites**

The system used to implement this is Ubuntu 18.04 LTS.

Before porting this repository to the main branch, it is advised that bazel-bin/main/lgshell is properly compiled and in working condition.

Clone this in the main (livehd) folder, preferably the same location as folders e.g. inou, bazel-bin, pass, main.
```bash
git clone 
```

Below is a list of Anaconda package dependencies for `LiveHD+Jupyter.ipynb`. Many of these packages are from `conda-forge` package channel. Specify the channel with flag `-c` when installing.

* xeus-cling (C++ Jupyter kernels)
* bash-kernel (Bash Jupyter kernel)
* ~~ipywidget (Python Interactive Notebook)~~
* graphviz-python (Python)

## **Running**
`LiveHD+Jupyter.ipynb` is compatible with both C++ and Python kernels.
1. Create a new virtual environment with Anaconda
```bash
conda create -n <envname>
```
2. Enter the virtual environment just created
```
source activate <envname>
```
3. Install the required packages in this virtual environment. 
```
conda install -c <channel> <package_name>
```
4. Open Jupyter Notebook `LiveHD+Jupyter.ipynb` 