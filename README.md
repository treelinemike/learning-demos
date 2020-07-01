# learning-demos
Machine learning demos

Download LATEST Anaconda installer for windows (will say Python 3.7): https://www.anaconda.com/products/individual#windows
Install Anaconda
Launch Anaconda prompt from windows start menu

`$ conda create --name ralpn-seg`
`$ conda activate ralpn-seg`

> conda install jupyter

> conda install tensorflow

> pip install --upgrade tensorflow      <-- This will update tensorflow to v2.2.0 or greater

> conda install pydot                   <-- This is where doing things in base environment failed

> conda install matplotlib

# Load MNIST, etc...
> conda install tensorflow-datasets     

> pip install -U tensorflow-datasets    <-- update to current version (maybe skip prev. call?)... this broke for me a bit, after updating and restarting jupyter it seems to be working now?

> conda install pillow                  <-- Python imaging library, forked... may not need

May also need this:
> conda install graphviz


Then find the graphviz path, probably something like c:\Users\f002r5k\.conda\pkgs\graphviz-2.38-hfd603c8_2\Library\bin\graphviz, and add it to system PATH
Trick for resetting path without rebooting:
> set PATH=C

Close anaconda prompt and open an new one. Check with 
> echo %PATH%


In prompt change to appropriate drive/folder
> D:
> ........

Launch Jupyter Notebook:
> jupyter notebook

Navigate in Jupyter browser to correct folder (need to have launched from the correct drive, etc.) 