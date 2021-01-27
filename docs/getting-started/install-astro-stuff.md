# Install these astronomy-specific python packages

There are several packages used in this research. The steps below walk you through install them.

# Installation instructions

The instructions below should work for all platforms...if you run into problems please let us know!

## Make an "environment" just for astro research 

Doing this creates a "virtual" copy of your python installation. If something goes wrong with that copy or it gets messed up or the setup changes a lot it is easy to delete the copy and start fresh.

To make the environment copy/paste this into your terminal and hit `Enter` to run it. You will be asked to confirm that you want to create the environment:

```
conda create -n astro_research python=3.8 astropy
```

You only need to make the environment once, but you will need activate it *every time you use the environment*.

## Activate your new environment 

Type this in the terminal and push `Enter` to activate the environment (i.e. make it the Pythn you are using):

```
conda activate astro_research
```

## Install astropy, its affiliated projects, and more

Copy and paste the long line below into your terminal and press enter to run it. After a couple of minutes you should get a prompt asking you to confirm that you want to install this stuff.

```
conda install -c conda-forge astropy astroquery ccdproc ginga ipywidgets bottleneck photutils matplotlib pandas gatspy pyyaml astrowidgets jupyterlab=2 jedi=0.17 ipympl nodejs
```

## Install an extension to make the Jupyter notebooks we use interactive

Once again, copy/paste into the terminal:

```
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```
