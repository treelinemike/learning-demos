# learning-demos
Machine learning demos

Download LATEST Anaconda installer for windows (will say Python 3.7): https://www.anaconda.com/products/individual#windows
Install Anaconda
Launch Anaconda prompt from windows start menu
> conda install tensorflow
> pip install --update tensorflow      <-- This will update tensorflow to v2.2.0 or greater
> conda install pydot

That may fail due to permissions. Not sure why. Maybe we need to do this in a new environment rather than base?
If it fails we can proceed by launching Anaconda power shell prompt by right clicking and running as administrator
> conda update -n base -c defaults conda

UGH! Try again, but do this in a new envronment, not the base environment...



----------  ALL OF THIS IF USING OLD KERAS WHICH DIDN'T RUN WITH PYTHON 3.7
To get up an running "quickly":
Remove existing versions of Python (for good measure, may not be necessary)
Download LATEST Anaconda installer for windows (will say Python 3.7): https://www.anaconda.com/products/individual#windows
Follow instructions for creating conda environments with Python 3.5: https://docs.anaconda.com/anaconda/user-guide/faq/#anaconda-faq-35

Then.... launch Anaconda PROMPT from windows menu and execute the following:
> conda create --name ralpn-seg python=3.5
> conda info --envs
> conda activate ralpn-seg

Install required packages:
> conda install jupyter
> conda install keras
> conda install pywin32
> conda install matplotlib=2.2.3 (need old version of matplotlib because of 'NoneType' object is not iterable error)

Install visualization tools
> conda install pydot
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