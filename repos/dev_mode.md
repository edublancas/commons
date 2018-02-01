# Installing __PROJECT_NAME__ in development mode

Replace __PROJECT_NAME__, __PACKAGE_NAME__, __PROJECT_URL__ and
__ROOT_FOLDER_NAME__

First, we need to install __PROJECT_NAME__ in develop mode.

Clone the repo:

```shell
git clone __PROJECT_URL__
```

Move to the folder containing the `setup.py` file and install the package in development mode:

```shell
cd __ROOT_FOLDER_NAME__
pip install --editable .
```

If you install it that way, you can modify the source code and changes will reflect whenever you import the modules (but you need to restart the session).

Make sure you can import the package and that it's loaded from the location where you ran `git clone`. First open a Python intrepreter:

```shell
python
```

And load the package you installed:

```python
import __PACKAGE_NAME__
__PACKAGE_NAME__
```

You should see something like this:

    path/to/cloned/repository


## Developing a package without restarting a session

If you use IPython/Jupyter run these at the start of the session to reload your packages without having to restart your session:

```python
%load_ext autoreload
%autoreload 2
```

