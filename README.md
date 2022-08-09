# pydap_notebooks
just some experiment notebooks for pydap


# Recipe to run notebooks

## Create a project folder (duh)

    mkdir pydap
    cd pydap

## Create a venv and activate it
    
    python -m venv venv
    source venv/bin/activate

## Install pydap

### Either directly from github

    pip install git+https://github.com/OPENDAP/pydap.git@dap4_beta


### Or clone the repository and install from local

    cd pydap
    git clone git@github.com:OPENDAP/pydap.git --branch dap4_beta
    pip install -e pydap/


## Run the notebooks
    
    pip install jupyterlab
    git clone git@github.com:NiklasPhabian/pydap_notebooks.git

NB: I could not get the above clone to work, but

	git clone https://github.com/NiklasPhabian/pydap_notebooks.git

did work. jhrg 8/9/22

Note; edit the user.config 

