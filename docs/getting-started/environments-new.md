# Python environments

A python environment is essentially a virtual copy of your main python installation. Environments are independent of each other, so you can make changes in one environment without affecting other environments.

Using `conda` or `mamba` is one way to manage environments. Python comes with `venv`, which is another way of managing environments. It doesn't matter which one you use, but these instructions will be for `conda`/`mamba`

## creating an environment

`mamba create -n play python=3.11`

## activate

Activating the environment makes it the Python installation you are using. When activated you should see the name of the environment somewhere in your command line prompt in parentheses (e.g. `(play)`).

`mamba activate play`

## deactivate

Use `mamba deactivate` to leave the environment.

## Removing an environment (not usually necessary)

If an environment gets messed up, or if you know you won't need the environment any more, or you just want to save some disk space, you cna delete the environment. This will not affect your code or anything, it only deletes the Python environment.

`mamba remove -n play --all --yes`