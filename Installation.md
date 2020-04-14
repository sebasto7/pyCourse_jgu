# Installation instructions 
To use a specific scientific package written for Python, you will often need to install specific versions of other (sub)packages. A nice way to organize all the packages and (sub)packages to not mix different version of them, is to create different environments. Each environment will have a specific group of packages inside. You can even decide which version of Python itself (2.7 or 3.7, for example) will be running with those packages. In this way, incompatibility issues between packages, previously installed in your computer, will be avoided.

Follow this instructions to install the required elements for our python for beginners course, create environments and install specific packages in them. Follow the instructions for your system.


## 1. Common. Anaconda installation
Installing Anaconda for using conda. "conda" is a package manager meaning that you can easily download, store and organize packages (collections of codes that someone wrote for achieving a certain set of tasks). Anaconda is a set of about a hundred packages including conda (our package manager). It is the most convenient way to use python and python packages.

go to: https://www.anaconda.com/distribution/#download-section
install the version for Python 3.7.

If you don’t want the hundreds of packages included with Anaconda, you can install Miniconda, a mini version of Anaconda that includes just conda, its dependencies, and Python.

go to: https://docs.conda.io/projects/continuumio-conda/en/latest/user-guide/install/index.html

Now, continue with 2.1, 2.2, or 2.3. 


### 2.1. Using Anaconda Navigator (User interface)
Open up "Anaconda Navigator" (You can search for it in the searchbar).
Many applications, including Jupyter notebooks, are availeble in the navigator by default, but you need to install them first.

Navigator is an easy, point-and-click way to work with packages and environments without needing to type conda commands in a terminal window. You can use it to find the packages you want, install them in an environment, run the packages, and update them, all inside Navigator.
1. In Navigator, click the Environments tab, then click the Create button. The Create new environment dialog box appears.
2. In the Environment name field, type a descriptive name for your environment (e.g., python_intro_course_environment), and select Python version 3.7.
3. In Navigator, click the Home tab, select your environment at "Application on", and click to INSTALL Jypyter Notebook.
4. LAUNCH Jupyter Notebook.

It should open up a browser which will show you some directories that are located in your computer. Here navigate to the directory where you downloaded our course material.

To learn much more,
go to: https://docs.anaconda.com/anaconda/navigator/


### 2.2. Using the terminal: Mac OS X
Open up "Terminal" (You can search for it in the searchbar). Here we will type commands in order to do some stuff. In this tutorial (also probably in your own terminal) the commands you will write will start with "$". Let's see if conda is installed by writing the following command:

*$conda*

press Enter and just after your typed command you will see: 

*'''
usage: conda [-h] [-V] command ...
conda is a tool for managing and deploying applications, environments and packages.
Options:
'''*

This means that you have successfully installed conda.

#### Jupyter notebook installation into a new environment
Now you will type things in the terminal in order to create a new environment and install the required packages in it. Type the following:

*$conda create -n python_intro_course_environment*

This will create a new environment named "python_intro_course_environment (name is determined with whatever follows the '-n' within that line of code). We now created the environment but we're not inside yet so let's go in this environment by  typing:

*$conda activate python_intro_course_environment*

Are we in? We can check it by looking at the leftmost part of the command line. It should show (python_intro_course_environment).

Now let's install Jupyter Notebook package. First let's search if there is any package named jupyter. 

*$conda search jupyter*

It will give us a bunch of different jupyter packages but we don't need to worry about which ones to install since conda takes care of that automatically. The command for installing a package with conda is "install".

*$conda install jupyter*

after that we can run jupyter notebook:

*$jupyter notebook*

It should open up a browser which will show you some directories that are located in your computer. Here navigate to the directory where you downloaded our course material.


### 2.3 Using the terminal: Windows 
