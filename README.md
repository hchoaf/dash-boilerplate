# Setting up Python & Jupyter


## Installing Anaconda/Python

We will be using *python version 3.8* for this workshop. We recommend using the Anaconda distribution to install Python and Jupyter.

**Using Anaconda** (Recommended)

Download the installer specific to your OS and follow the steps on the Anaconda website

https://docs.anaconda.com/anaconda/install/


## Setup

#### Download this repository and run all the commands from the root folder

### Creating a virtual environment

1. We recommend creating a virtual environment to add all the dependencies. To create a new virtual environment run:
``` conda create --name cfg-dash  ```

2. Verify that the new environment was installed correctly: ``` conda env list ``` You should see an env called cfg-dash

3. Activate the new environment: ``` conda activate cfg-dash ```

4. Anaconda should install all necessary dependencies but if not please install all required dependencies from the requirements.txt file provided: ``` pip install -r requirements.txt ```

5. Add the new virtual env to the jupyter kernel: ``` python -m ipykernel install --user --name=cfg-dash ```


### Launching a jupyter notebook

- Within your conda env run: ``` jupyter notebook ```

- This will print some information about the notebook server in your terminal, including the URL of the web application (by default, http://localhost:8888):

``` 
[I 08:58:24.417 NotebookApp] Serving notebooks from local directory: /Users/sagar
[I 08:58:24.417 NotebookApp] 0 active kernels
[I 08:58:24.417 NotebookApp] The Jupyter Notebook is running at: http://localhost:8888/
[I 08:58:24.417 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
```

It will then open your default web browser to this URL and you will see this notebook dashboard.


Click on the notebook cfg-dash-boilerplate and you should see the following:



1. Make sure that the notebook shows trusted on the top right (else click on where it says "Untrusted" and select "Trust")
2. Ensure that the kernel on the top right shows cfg-dash. If not then click on Kernel -> Change Kernel -> cfg-dash


https://jupyter.readthedocs.io/en/latest/install/notebook-classic.html
https://jupyter.readthedocs.io/en/latest/running.html#running

## Conclusion

Congrats, you're done! That's all the pre-work you need for the Dash and Jupyter Workshop

If you're curious and want to read more on the tools we're gonna be using, you can visit these links:

- Jupyter notebook basics: https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Notebook%20Basics.html
- Plotly graphing library: https://plotly.com/python/
- Dash User Guide: https://dash.plotly.com/
