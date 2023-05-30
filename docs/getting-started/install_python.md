# Install Python

## Install the miniconda python distribution

There are several ways to install python. For research it is convenient to have an installation that:

+ Includes several scientific python packages.
+ Does not interfere with any other python installation you already have (e.g. for the intro computer science courses or vpython).
+ Works on Windows, Mac, or Linux.

The best option currently is the [miniforge python distribution](https://github.com/conda-forge/miniforge).

Download anaconda now and install it.

**If you are using python for some other purpose**, like a computer science course, be sure to unselect the option during installation that makes anaconda's python your default python. If you accidentally forget to do that it is easy to fix later.

## Try your installation

1. Open a terminal window
    + On **Windows**: Click the start menu, then start typing "Anaconda Prompt" (but without the quotes) and select `Anaconda Prompt`
    + On **Mac**, type CMD-space to bring up the search box and start typing "Terminal" (but without the quotes) and select `Terminal`.
2. Type `conda list` in the terminal and then hit `Enter`. You should see a  list of installed python packages.

## Did you see an error instead of a list?

That is almost certainly because miniconda wasn't made your default python installation (which is the right choice if you are using python for another course).

Each time you want to use miniconda, open a terminal window and type (or copy/paste) the command below appropriate for your operating system.

## Configure a couple of extra anaconda channels for astronomy-related packages

The two channels you definitely want to add are `conda-forge` and `astropy`. Do that like this:

```bash
conda config --append channels astropy
conda config --append channels conda-forge
```
