**Pre-requites:**
Google Account
Google Cloud Platform Project
Google Cloud Linux VM 
PuttyGen

**The project steps are as follows:**

1. Created a VM instance in GCP under KBS-Skin-Lesion.

2. Launched a Google Cloud Linux VM instance to install Anaconda for Python development using the below commands:

    a. First, we start and connect to VM instance via SSH
    
    b. We run the following commands to update system packages and the core dependencies for Anaconda.
    
        $ sudo apt-get update
        $ sudo apt-get install bzip2 libxml2-dev
        
    c. To install a full Anaconda distribution:
    
        $ wget https://repo.anaconda.com/archive/Anaconda3-2018.12-Linux-x86_64.sh
        $ bash Anaconda3–2018.12-Linux-x86_64.sh
        
    d. After installation has completed, we can remove the shell script to save disk space.
    
        $ rm Anaconda3–2018.12-Linux-x86_64.sh
        
    e. Now we reinitialise the shell to recognise the conda command.
    
        $ source .bahsrc
        
    f. To verify that everything is installed properly.
    
        $ python --version
        $ which python
        $ which conda
        $ conda list conda$
        
**Here are the steps to work with the data and train our model**

The steps for preprocessing and dashboard can be found [here](https://github.com/Group13KBS/FinalProject/blob/master/Notebooks/preprocessing.ipynb)

The steps to train the model and to predict skin cancer based on images can be found [here](https://github.com/Group13-KBS/FinalProject/blob/master/Notebooks/Skin_Cancer.ipynb)
