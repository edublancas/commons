# Developing a Python package

Clone the repo:

```
git clone https://github.com/edublancas/sklearn-evaluation
```

Move to the folder containing the `setup.py` file (usually in the root folder) and install the package in development mode:

```
python setup.py develop
```

If you install it that way, you can modify the source code and changes will reflect wherever you import the modules (you need to restart the session).

Make sure you can import the package and that it's loaded from the location where you ran `git clone`. First open a Python intrepreter:

```
python
```

And load the package you installed:

```
import sklearn_evaluation
```

You should see something like this:

```
path/to/cloned/repository
```

## Developing a package without restarting a session

If you use IPython/Jupyter run these to reload your package without having to restart your session:

```python
%load_ext autoreload
%autoreload 2
```
