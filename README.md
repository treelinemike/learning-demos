# learning-demos

Machine learning demos in Python (Jupyter notebooks)

1. Function approximation. Artificial neural networks are just function approximators; they try to learn the nonlinear mapping between two sets from data. When the output set is finite and discrete this is classification (i.e. network assigns a label to each input element). When the output set is continuous the problem is regression (i.e. assign a continuous scalar value to each input element. In this example we perform regression trying to learn the L2 norm for inputs in R^2.

2. Basic 2D CNN with MNIST handwriting dataset. We try to learn how to read handwritten numbers 0-9.

#### 'Toolchain' installation on Windows

Download LATEST Anaconda installer for windows (will say Python 3.7): https://www.anaconda.com/products/individual#windows

Install Anaconda

Launch Anaconda prompt from windows start menu

#### Create and activate an environment (don't work directly in base environment)

```
$ conda create --name ralpn-seg
$ conda activate ralpn-seg
```

#### install required packages

```
$ conda install jupyter
$ conda install tensorflow
$ pip install --upgrade tensorflow      <-- This will update tensorflow to v2.2.0 or greater
$ conda install pydot                   <-- This is where doing things in base environment failed
$ conda install matplotlib
$ conda install tensorflow-datasets     <-- MNIST handwriting dataset, etc. 
$ pip install -U tensorflow-datasets    <-- update to current version (maybe skip prev. call?)... this broke for me a bit, after updating and restarting jupyter it seems to be working now?
```

#### May also need:

```
$ conda install pillow                  <-- Python imaging library, forked... may not need
$ conda install graphviz
```

Then find the graphviz path, probably something like c:\Users\f002r5k\.conda\pkgs\graphviz-2.38-hfd603c8_2\Library\bin\graphviz, and add it to system PATH

Trick for resetting path without rebooting:

`$set PATH=C`

Close anaconda prompt and open an new one. Check with 

`$ echo %PATH%`

#### Other notes

In prompt change to appropriate drive/folder

`$ D:`

Launch Jupyter Notebook:

`$ jupyter notebook`

Navigate in Jupyter browser to correct folder (need to have launched from the correct drive, etc.) 