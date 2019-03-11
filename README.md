# IIT-AGNE-Workshop
This repository consists of materials used for IIT AGNE Workshop. Below are the steps to install H2O to start with. 

## Downloading & Installing H2O
This section describes how to download and install the latest stable version of H2O. These instructions are also available on the <a href="http://h2o-release.s3.amazonaws.com/h2o/latest_stable.html">H2O Download page</a>.

Note: To download the nightly bleeding edge release, go to <a href="https://h2o-release.s3.amazonaws.com/h2o/master/latest.html">h2o-release.s3.amazonaws.com/h2o/master/latest.html</a>. Choose the type of installation you want to perform (for example, “Install in Python”) by clicking on the tab.


### Install in Python
Run the following commands in a Terminal window to install H2O for Python.

Install dependencies (prepending with sudo if needed):
```
pip install requests
pip install tabulate
pip install "colorama>=0.3.8"
pip install future
```

Note: These are the dependencies required to run H2O. A complete list of dependencies is maintained in the following file: https://github.com/h2oai/h2o-3/blob/master/h2o-py/conda/h2o/meta.yaml.

Run the following command to remove any existing H2O module for Python.
```
pip uninstall h2o
Use pip to install this version of the H2O Python module.
pip install -f http://h2o-release.s3.amazonaws.com/h2o/latest_stable_Py.html h2o
```

Note: When installing H2O from pip in OS X El Capitan, users must include the --user flag. For example:

```
pip install -f http://h2o-release.s3.amazonaws.com/h2o/latest_stable_Py.html h2o --user
```
Optionally initialize H2O in Python and run a demo to see H2O at work.
```
python
import h2o
h2o.init()
h2o.demo("glm")
```
