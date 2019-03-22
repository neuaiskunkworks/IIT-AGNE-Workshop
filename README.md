# IIT-AGNE-Workshop
This repository consists of materials and instructions that will be used for IIT AGNE Workshop. Below are the steps for setting up your computer.

We will do this in two steps.
  1. Setup Python Environment with Anaconda
  2. Install Python H2O Library

## Step 1: Python Environment Setup
Python will be our primary programming langauge for this workshop. We can install python from various distributors, but we will use Anaconda.

##### What is Anaconda?
Anaconda is a free and open-source distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment.

##### Why Anaconda?
While original Python distibution gives you only a basic platform and you have to install your desired libraries manually, Anaconda's Python distibution provides tons of libraries out of the box. With Anaconda, all your important Mathematics, Science and Engineering python libraries are pre-installed.

#### Installing Python with Anaconda
  1. Visit [Anaconda Website](https://www.anaconda.com/download) and download the latest Python 3.x version of Anaconda.
  2. Run the downloaded installer.

## Step 2: Install Python H2O Library
**We will use H2O library for building our predictive analytics model.**

This section describes how to download and install the latest stable version of H2O. The instructions are also available on the [H2O Download page](http://h2o-release.s3.amazonaws.com/h2o/latest_stable.html).

Before installing H2O, we need to install few dependency libraries.
#### 1. Install Python Dependency Library
Run the following commands in a Terminal window to install H2O for Python.

- Install dependencies (prepending with sudo if needed):
```
pip install requests
pip install tabulate
pip install "colorama>=0.3.8"
pip install future
```

Note: These are the dependencies required to run H2O. A complete list of dependencies is maintained in the following file: https://github.com/h2oai/h2o-3/blob/master/h2o-py/conda/h2o/meta.yaml.

#### 2. Install Python H2O Library
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

#### 3. Test H2O installation
- Optionally initialize H2O in Python and run a demo to see H2O at work.
```
python
import h2o
h2o.init()
h2o.demo("glm")
```


Kindly download the file from the below link for the workshop if required.

https://drive.google.com/file/d/1q1fiYCDuEEo-iWiciOH59ppntYIb8OF2/view?usp=sharing


## Want to join us Skunkworks? and contribute to the Skunkworks Projects?
Kindly have a look <a href="https://github.com/skunkworksneu/How-to-be-a-Skunk">here</a>
