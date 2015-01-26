# Install these astronomy-specific python packages

We use these packages regularly:

+ [astropy](http://astropy.org): installed with anaconda, it includes a ton of basic functionality.
+ [ccdproc](http://ccdproc.readthedocs.org): For reducing (calibrating) CCD data
+ [reducer](https://github.com/mwcraig/reducer): IPython notebook interface to `ccdproc`.
+ [msumastro](http://msum-astro.readthedocs.org): Package for conveniently manipulating directories of images.

# Installation instructions

Though [reducer](https://github.com/mwcraig/reducer) is given as the example below, any of the programs above can be installed the same way (except astropy...do **not** do `pip install astropy` in anaconda).

## Mac/Linux

You can install [reducer](https://github.com/mwcraig/reducer) and all of its dependencies with

```
$ pip install --pre reducer
```

## Windows

Though `pip` might work, you are better off trying to install conda package instead because they avoid the need for you to compile anything:

```
> conda install -c mwcraig reducer
```

