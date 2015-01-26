# Calibate your images with reducer

## Before you start

Make sure [reducer](https://github.com/mwcraig/reducer) is installed. To check, type this in a terminal window:

```
conda list reducer
```

If you see something like this you are ready to go:

```
# packages in environment at ....:
#

reducer                   0.1.deva592334            <pip>
```


If, instead, you see something like this:

```
# packages in environment at ...:
#
```
then you need to install reducer. This should work:

```
conda install -c mwcraig reducer
```

## Using reducer

1. Make a new folder -- this is where the calibrated images will end up.
2. Open a terminal window or powershell.
3. Change directory in the terminal into the folder you made.
4. Type `reducer` in the terminal (then hit enter).
5. Type `ipython notebook` in the terminal (then hit enter).
6. Walk through the reduction notebook using either the default data that comes with reducer.
