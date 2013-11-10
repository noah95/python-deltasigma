python-deltasigma
===============

The MATLAB Delta Sigma Toolbox with 0% MATLAB and a lot more Python.

The **python-deltasigma** project aims to provide **a 1:1 Python replacement** of Richard 
Schreier's *excellent* **[MATLAB Delta Sigma Toolbox](http://www.mathworks.com/matlabcentral/fileexchange/19-delta-sigma-toolbox)**, upon which it is very heavily based. The original toolbox is also known as *delsig* or *delsigma*.

### Status

This project is at **a very early stage**. Not all functionality has been ported and currently *the example files do not run*. Take a look to files.ods for the current status. 

**NEWS!** To have an idea of the currently implemented functionality, take a look at **[these preliminary results.](http://nbviewer.ipython.org/7251113)**, which showcases almost all `dsexample1.m`.

### How to contribute

Pull requests are welcome!

There are only a few *guidelines*, which can be overridden every time it is reasonable to do so:

* Please try to follow PEP8. Except you are free to indent with tabs or spaces as you please (but please stick with your choice). 

* Try to keep the functions signature identical. Parameters with `NaN` default values have their default value replaced replaced with None. 

* If a function has a varible number of return values, its Python port should implement the maximum number of return values,

## Dependencies

Using **python-deltasigma** requires:

#### 1. **numpy** and **scipy** 

**numpy** and **scipy** can be installed through the steps described below.

On a Debian Linux system:

```
 # aptitude install python-numpy python-scipy python-matplotlib
```

Or, on a generic platform:

```
# pip install numpy scipy
```

More information on the [scipy install page](http://www.scipy.org/install.html).

#### 2. matplotlib

**[matplotlib](http://matplotlib.org/)** is used for plotting and it is also very useful for visually inspecting your data.


#### 3. Extras

Building the documentation requires the **[sphinx](http://sphinx-doc.org/)** package.

If you plan to run the provided unit tests, then you should install **[setuptools](https://pypi.python.org/pypi/setuptools)**, used to access the reference function outputs. Testing *can* be automated with **[nose](https://pypi.python.org/pypi/nose/)**, issuing `$ nosetests -v pydelsigma/*.py`.

## Licensing and copyright notice

All original MATLAB code is Copyright (c) 2009, Richard Schreier. See the LICENSE file for the licensing terms.

The Python here provided is a derivative work from the above toolkit and subject to the same license terms.

The Python code is Copyright 2013, Giuseppe Venturini and the python-deltasigma contributors.

MATLAB is a registered trademark of The MathWorks, Inc.
