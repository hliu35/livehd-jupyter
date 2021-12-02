# Jupyter Instructions

## **Prerequisites**

The system used to implement this is Ubuntu 18.04 LTS.

Before porting this repository to the main branch, it is advised that bazel-bin/main/lgshell is properly compiled and in working condition.

Clone this in the main (livehd) folder, preferably the same location as folders e.g. inou, bazel-bin, pass, main.
```bash
cd livehd
git clone https://github.com/hliu35/livehd-jupyter
```

Below is a list of Anaconda package dependencies for `LiveHD+Jupyter.ipynb`. Many of these packages are from `conda-forge` package channel. Specify the channel with flag `-c` when installing.

* xeus-cling (optional, C++ Jupyter kernels)
* bash-kernel (optional, Bash Jupyter kernel)
* ~~ipywidget (Python Interactive Notebook)~~
* graphviz-python (Python)

## **Running**
`LiveHD+Jupyter.ipynb` is compatible with both C++ and Python kernels.
1. Create a new virtual environment with Anaconda
```
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

Start a Jupyter Notebook server session by running
```
jupyter notebook
```
Or opening the file in IDE such as Visual Studio Code