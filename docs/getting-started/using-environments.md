# Environments

`conda` has a concept called an environment that is essentially an "duplicate" installation of python with as many (or as few) things in it as you want.

To create one, do, at the command line in a terminal, `conda create -n name_of_your_env list_of_packages_you_want`. To make an environment called `astro` with `ccdproc`, `photutils`, `ipywidgets` and all of their dependencies, do:

```bash
conda create -n astro ccdproc photutils ipywidgets
```
