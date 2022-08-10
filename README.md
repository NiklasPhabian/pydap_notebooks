# pydap_notebooks
just some experiment notebooks for pydap


# Recipe to run notebooks

## Create a project folder (duh)

    mkdir pydap
    cd pydap

## Create a venv and activate it
    
    python3 -m venv venv
    source venv/bin/activate

## Install pydap

### Either directly from github

    pip3 install git+https://github.com/OPENDAP/pydap.git@dap4_beta
    
NB: This worked for me at home, but not on my office computer. jhrg 8/10/22 

### Or clone the repository and install from local

    cd pydap # not sure this is needed. jhrg 8/10/22
    # git clone git@github.com:OPENDAP/pydap.git --branch dap4_beta didn't work at home jhrg 8/10/22
    git clone https://github.com/OPENDAP/pydap.git --branch dap4_beta
    pip3 install -e pydap/


## Run the notebooks
    
    pip3 install jupyterlab
    git clone git@github.com:NiklasPhabian/pydap_notebooks.git

NB: I could not get the above clone to work, but

	git clone https://github.com/NiklasPhabian/pydap_notebooks.git

did work. jhrg 8/9/22

Note; edit the user.config 

