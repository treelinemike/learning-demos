# learning-demos
Machine learning demos

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

In prompt change to appropriate drive/folder
> D:
> ........

Launch Jupyter Notebook:
> jupyter notebook

Navigate in Jupyter browser to correct folder (need to have launched from the correct drive, etc.) 