# IIT-AGNE-Workshop
This repository consists of materials and instructions that will be used for IIT AGNE Workshop. Below are the steps to for setting up your computer.

## Python Environment Setup
### Introduction
This readme will help you setup the initial python environment. While there are many ways and resources to get started with, there usually comes a point when these techniques fail if you don't have the right set of tools to begin with. To help you better understand, imagine you want to grow a tree in your backyard. Well, you have this tree sapling along with sickle to plough the soil and the watering can. Don't you think we are missing something..? What about the type of soil required for growing it, or the enivronment? We need the right fertilizers or pesticides to keep it safe from bugs. Likewise, when it comes to programming in general, we need to make sure we have the right set of environment along with the relevant libraries to make the entire system to function efficiently.

This will help you setup your environment for getting started with python and data science journey.

##### Contents:

1. Installing Anaconda --> Windows, MAC
2. Installing libraries and packages

#### 1. Installing Anaconda
##### What is Anaconda?
Anaconda is a free and open-source distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment.

##### Why Anaconda?
While traditional Python gives you just a basic platform where you have to install your desired packages manually ( this even does not have NumPy and Pandas installed), Anaconda gives you just everything. I mean it has the most useful packages for Mathematics, Science and Engineering already installed for you.

Removes bottlenecks involved in installing the right packages while taking into considerations their compatibility with various other packages as might be encountered while using pip.

There is no risk of messing up required system libraries

Must I add that it has upto 720 open source packages, most of which are not in the pip repo?

##### Windows
###### Installing Anaconda
- Visit <a href="https://www.anaconda.com/download">Anaconda Website</a> and download the 64bit versioin if you have 64 bit machine or 32bit if you have a 32 bit machine. Download the latest Python 3. version of Anaconda. This will download the .exe** file on your computer.

- Double click the installer to launch the Anaconda SetUp. NOTE: To prevent permission errors, do not launch the installer from the Favorites folder.

NOTE: If you encounter issues during installation, temporarily disable your anti-virus software during install, then re-enable it after the installation concludes. If you installed for all users, uninstall Anaconda and re-install it for your user only and try again.

1. Click Next.
2. Read the licensing terms and click “I Agree”.
3. Select an install for “Just Me” unless you’re installing for all users (which requires Windows Administrator privileges) and click Next.
4. Select a destination folder to install Anaconda and click the Next button. See FAQ. NOTE: Install Anaconda to a directory path that does not contain spaces or unicode characters. NOTE: Do not install as Administrator unless admin privileges are required.
5. Choose whether to add Anaconda to your PATH environment variable. We recommend not adding Anaconda to the PATH environment variable, since this can interfere with other software. Instead, use Anaconda software by opening Anaconda Navigator or the Anaconda Prompt from the Start Menu.
6. Choose whether to register Anaconda as your default Python. Unless you plan on installing and running multiple versions of Anaconda, or multiple versions of Python, accept the default and leave this box checked.
7. Click the Install button. If you want to watch the packages Anaconda is installing, click Show Details.
8. Click the Next button.
9. Optional: To install VS Code, click the Install Microsoft VS Code button. After the install completes click the Next button. Or to install Anaconda without VS Code, click the Skip button.

NOTE: Installing VS Code with the Anaconda installer requires an internet connection. Offline users may be able to find an offline VS Code installer from Microsoft.

1. After a successful installation you will see the “Thanks for installing Anaconda” dialog box.
2. If you wish to read more about Anaconda Cloud and how to get started with Anaconda, check the boxes “Learn more about Anaconda Cloud” and “Learn how to get started with Anaconda”. Click the Finish button.
3. After your install is complete, verify it by opening Anaconda Navigator, a program that is included with Anaconda: from your Windows Start menu, select the shortcut Anaconda Navigator. If Navigator opens, you have successfully installed Anaconda. If not, check that you completed each step above, then see our Help page.

Your setup is now complete. To test the installation, type

```conda list```

Also, since you need to update your anaconda installation to have all the latest versions of the libraries. Hence run

```conda update conda```

This will display a list of installed libraries pre-installed by anaconda. The list is quite exhaustive and you can check out the various data libraries given here.

##### MAC
###### Installing Anaconda
1. Visit <a href="https://www.anaconda.com/download">Anaconda Website</a> and download the 64bit versioin if you have 64 bit machine or 32bit if you have a 32 bit machine. Download the latest Python 3. version of Anaconda. This will download the .sh** file on your computer.
2. Double-click the downloaded file and click continue to start the installation..
3. Answer the prompts on the Introduction, Read Me and License screens.
4. Click the Install button to install Anaconda in your home user directory (recommended)
5. OR, click the Change Install Location button to install in another location (not recommended).
On the Destination Select screen, select Install for me only.
NOTE: If you get the error message “You cannot install Anaconda in this location,” reselect Install for me only.

6. Click the continue button.
7. Optional: To install VS Code, click the Install Microsoft VS Code button. After the install completes click the Continue button.
Or to install Anaconda without VS Code, click the Continue button.

NOTE: Installing VS Code with the Anaconda installer requires an internet connection. Offline users may be able to find an offline VS Code installer from Microsoft.

8. A successful installation is displayed on the screen
9. After your install is complete, verify it by opening Anaconda Navigator, a program that is included with Anaconda: from Launchpad, select Anaconda Navigator. If Navigator opens, you have successfully installed Anaconda.


### Installing libraries and packages
##### What is Conda and pip?
Both Conda and pip are packaging tool consisting of various packages. Pip is a package manager used for installing and managing various python packages and hence is a package management system. Whereas Conda is a package management system as well as environment management system that runs on various platforms. It aims to do more than what pip does; handle library dependencies outside of the Python packages as well as the Python packages themselves. Conda also creates a virtual environment, like virtualenv does.

Because Conda introduces a new packaging format, you cannot use pip and Conda interchangeably; pip cannot install the Conda package format. You can use the two tools side by side (by installing pip with conda install pip) but they do not interoperate either.

##### INSTALLING CONDA PACKAGES:
- To list and check for all of the packages in the active environment:

```conda list```

- The package installs into the current environment:

```conda install Package_Name```

- To install a specific version of a package:

```conda install Package_Name=0.15.0```

- To install multiple packages at once:

```conda install PackageName1 PackageName2```

NOTE: It is best to install all packages at once, so that all of the dependencies are installed at the same time.

- To install multiple packages at once and specify the version of the package:

```conda install PackageName1=0.15.0 PackageName2=7.26.0```

- To update a specific package:

```conda update Package_Name```

- To update Python:

```conda update python```

- To update conda itself:

```conda update conda```

NOTE: Conda updates to the highest version in its series, so Python 2.7 updates to the highest available in the 2.x series and 3.6 updates to the highest available in the 3.x series.

- To remove a package in an environment:

```conda remove -n env_path Package_Name```

- To remove a package in the current environment:

```conda remove Package_Name```

- To remove multiple packages at once:

```conda remove PackageName1 PackageName2```

- To confirm that a package has been removed:

```conda list```

##### INSTALLING NON-CONDA PACKAGES :
If a package is not available from conda or Anaconda.org, you may be able to find and install the package with another package manager like pip.

Pip packages do not have all the features of conda packages, and we recommend first trying to install any package with conda. If the package is unavailable through conda, try installing it with pip. The differences between pip and conda packages cause certain unavoidable limits in compatibility, but conda works hard to be as compatible with pip as possible.

NOTE: Both pip and conda are included in Anaconda and Miniconda, so you do not need to install them separately.

NOTE: Conda environments replace virtualenv, so there is no need to activate a virtualenv before using pip.

It is possible to have pip installed outside a conda environment or inside a conda environment.

To gain the benefits of conda integration, be sure to install pip inside the currently active conda environment, and then install packages with that instance of pip. The command 'conda list' shows packages installed this way, with a label showing that they were installed with pip.

You can install pip in the current conda environment with the command 'conda install pip'.

If there are instances of pip installed both inside and outside the current conda environment, the instance of pip installed inside the current conda environment is used.

To install a non-conda package:

Activate the environment where you want to put the program:

On Windows, in your Anaconda Prompt, run activate .
On macOS and Linux,in your Terminal window, run source activate .
- To use pip to install a program such as See, in your Terminal window or an Anaconda Prompt, run:

```pip install see```

- To verify the package was installed, in your Terminal window or an Anaconda Prompt, run:

```conda list```

NOTE: If the package is not shown, install pip and try these commands again.

- Upgrading pip

```conda update pip```

- Checking version of pip

```pip --version```

- Installing a package

```pip install Package_Name```

- Check for the files installed for a package

```pip show --files Package_Name```

- List installed packages

```pip list```

- List uptodate packages

```pip list --uptodate```

- Check for outdated files

```pip list --outdated```

- List packages that are not dependencies of other packages. Can be combined with other options

```pip list --outdated --not-required```

- Upgrading a package

```pip install --upgrade Package_Name```

- Uninstalling a package

```pip uninstall Package_Name```


## Downloading & Installing H2O
This section describes how to download and install the latest stable version of H2O. These instructions are also available on the <a href="http://h2o-release.s3.amazonaws.com/h2o/latest_stable.html">H2O Download page</a>.

Note: To download the nightly bleeding edge release, go to <a href="https://h2o-release.s3.amazonaws.com/h2o/master/latest.html">h2o-release.s3.amazonaws.com/h2o/master/latest.html</a>. Choose the type of installation you want to perform (for example, “Install in Python”) by clicking on the tab.


### Install in Python
Run the following commands in a Terminal window to install H2O for Python.

- Install dependencies (prepending with sudo if needed):
```
pip install requests
pip install tabulate
pip install "colorama>=0.3.8"
pip install future
```

Note: These are the dependencies required to run H2O. A complete list of dependencies is maintained in the following file: https://github.com/h2oai/h2o-3/blob/master/h2o-py/conda/h2o/meta.yaml.

- Run the following command to remove any existing H2O module for Python.
```
pip uninstall h2o
Use pip to install this version of the H2O Python module.
pip install -f http://h2o-release.s3.amazonaws.com/h2o/latest_stable_Py.html h2o
```

Note: When installing H2O from pip in OS X El Capitan, users must include the --user flag. For example:

```
pip install -f http://h2o-release.s3.amazonaws.com/h2o/latest_stable_Py.html h2o --user
```
- Optionally initialize H2O in Python and run a demo to see H2O at work.
```
python
import h2o
h2o.init()
h2o.demo("glm")
```
