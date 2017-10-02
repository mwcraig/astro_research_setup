# Install these astronomy-specific python packages

We use these packages regularly:

+ [astropy](http://astropy.org): installed with anaconda, it includes a ton of basic functionality.
+ [ccdproc](http://ccdproc.readthedocs.org): For reducing (calibrating) CCD data
+ [reducer](https://github.com/mwcraig/reducer): IPython notebook interface to `ccdproc`.
+ [msumastro](http://msum-astro.readthedocs.org): Package for conveniently manipulating directories of images.

# Installation instructions

The instructions below should work for all platforms...if you run into problems please let us know!

## Install astropy and affiliated projects

```
conda install ccdproc photutils ipywidgets
```

Note: all of the astropy-related packages are also available via pip. `conda` avoids compiling on Windows.

## Install the remaining software

You can install [reducer](https://reducer.readthedocs.org) and all of its dependencies with

```
pip install msumastro reducer
```
