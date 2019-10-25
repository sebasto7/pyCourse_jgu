# Installation instructions 
In this tutorial you'll learn how to install the required elements for our python for beginners course. Follow the instructions for your system.

## Mac OS X

### Anaconda installation
Installing Anaconda for using conda. "conda" is a package manager meaning that you can easily download, store and organize packages (collections of codes that someone wrote for achieving a certain set of tasks). Anaconda is a set of about a hundred packages including conda (our package manager). It is the most convenient way to use python and python packages.

go to: https://www.anaconda.com/distribution/#download-section
install the version for Python 3.7.

Open up "Terminal" (You can search for it in the searchbar). Here we will type commands in order to do some stuff. In this tutorial (also probably in your own terminal) the commands you will write will start with "$". Let's see if conda is installed by writing the following command:

$conda

press Enter and just after your typed command you will see: 
'''
usage: conda [-h] [-V] command ...

conda is a tool for managing and deploying applications, environments and packages.

Options:
'''
This means that you have successfully installed conda.

### Jupyter notebook installation into a new environment
Now you will type things in the terminal in order to create a new environment and install the required packages in it. Type the following:

$conda create -n python_intro_course_environment

This will create a new environment named "python_intro_course_environment (name is determined with whatever follows the '-n' within that line of code). We now created the environment but we're not inside yet so let's go in this environment by  typing:

$conda activate python_intro_course_environment

Are we in? We can check it by looking at the leftmost part of the command line. It should show (python_intro_course_environment).

Now let's install Jupyter Notebook package. First let's search if there is any package named jupyter. 

$conda search jupyter

It will give us a bunch of different jupyter packages but we don't need to worry about which ones to install since conda takes care of that automatically. The command for installing a package with conda is "install".

$conda install jupyter

after that we can run jupyter notebook:

$jupyter notebook

It should open up a browser which will show you some directories that are located in your computer. Here navigate to the directory where you downloaded our course material.


## Windows 
