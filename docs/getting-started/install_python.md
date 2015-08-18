# Install the anaconda python distribution

There are several ways to install python. For research it is convenient to have an installation that:

+ Includes several scientific python packages.
+ Does not interfere with any other pythoninstallation you already have (e.g. for the intro computer science courses or vpython).
+ Works on Windows, Mac, or Linux.

The best option currently is the [anaconda python distribution](http://continuum.io/downloads).

Download anaconda now and install it (the python 2.7 version, which is the default, or 3.4). **If you are using python for some other purpose**, like a computer science course, be sure to unselect the option during installation that makes anaconda's python your default python. If you accidentally forget to do that it is easy to fix later.

# Try your installation

1. Open a terminal window (see the [instructions here](http://cli.learncodethehardway.org/book/ex1.html) for your platform)
2. Type `conda list` in the terminal and then hit `Enter`. You should see a long list of installed python packages.

## Did you see an error instead of a list?

That is almost certainly because anaconda wasn't made your default python installation (which is the right choice if you are using python for another course).

Each time you want to use anaconda, open a terminal window and type (or copy/paste) the command below appropriate for your operating system.

### Mac/Linux

```bash
export PATH=$PATH:~/anaconda/bin
```

### Windows (powershell)

```
$env:Path = $env:Path + ";" + "$HOME\AppData\Local\Continuum\Anaconda" + ";" + "$HOME\AppData\Local\Continuum\Anaconda\Scripts"
```

Note: to paste in powershell, just right-click with your mouse.
