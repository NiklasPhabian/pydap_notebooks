# pydap_notebooks
Experimental notebooks for pydap with DAP4

# Recipe to run notebooks in a conda environment
See the later section for an example using Python venv

## Create a project folder (duh)

    mkdir pydap-demo
    cd pydap-demo

## Using conda

### Make a conda environment that includes numpy and jupyter-lab


    conda create --name pydap_test
    conda activate pydap_test
    
    conda install numpy
    conda install jupyterlab

### Get pydap and the pydap notebooks

    git clone https://github.com/OPENDAP/pydap --branch dap4_beta
    git clone https://github.com/NiklasPhabian/pydap_notebooks.git

### Install pydap using pip3 from the github repo that was just cloned

    pip3 install -e pydap/

### To get NASA Cloud URLs to work...
You need to make a user.config file with credentials for the NASA
Earthdata Cloud environment. Do this by copying the file
"user.config\_edit\_and\_rename\_no\_commit user.config"
to "user.config". Make sure that the "user.config" file is not
added/commited to git/github. That will expose your earthdata login
credentails to the world since the pydap\_notebook is world readable.

    cd pydap_notebooks
    cp user.config_edit_and_rename_no_commit user.config
    emacs user.config

### Start jupyter-lab
Maybe do this in a separate shell... your call, but in that case cd to
the pydap-demo directory

    jupyter-lab

Click on the pydap\_notebooks directory and run the pydap\_demo notebook.

## Using venv and pip3

### Create a venv and activate it
    
    python3 -m venv venv
    source venv/bin/activate

### Clone and Install pydap

    git clone https://github.com/OPENDAP/pydap.git --branch dap4_beta
    pip3 install -e pydap/

### Install jupyterlap the notebooks
    
    pip3 install jupyterlab
	git clone https://github.com/NiklasPhabian/pydap_notebooks.git

Now, goto _To get NASA Cloud URLs to work_ to set up NASA Earthdata
login credentials and run the demo notebook.

