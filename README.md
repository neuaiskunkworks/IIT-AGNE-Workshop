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
Visit <a href="https://www.anaconda.com/download">Anaconda Website</a> and download the 64bit versioin if you have 64 bit machine or 32bit if you have a 32 bit machine. Download the latest Python 3. version of Anaconda. This will download the .exe** file on your computer.

##### MAC
###### Installing Anaconda
Visit <a href="https://www.anaconda.com/download">Anaconda Website</a> and download the 64bit versioin if you have 64 bit machine or 32bit if you have a 32 bit machine. Download the latest Python 3. version of Anaconda. This will download the .sh** file on your computer.

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
