
# PyCon Nove Beginner's Day

All the materials of this tutorial is available in Jupyter notebook
format.

To have a sneak peak of what a Jupyter notebook is, jump to the
<a href="#notebook">Notebook format</a> section.

Before using the notebooks please follow the
<a href="#installation">installation guide</a> to install
`Python` according to your operating system.

<a name="installation"></a>
# Installation Guides

This guide goes over the proper installation of Python for development purposes.

## Python 3 Installation Guides

### Python 3 on Linux

Python is already installed in most of the Linux distributions.
So, in principle, you should be already done.

To see which version of Python 3 you have installed,
open a command prompt and run:

```bash
$ python3 --version
```

If you are using Ubuntu 16.10 or latest, then you can easily install
Python 3.6 with the following commands:

```bash
$ sudo apt-get update
$ sudo apt-get install python3.6
```

If you’re using another version of Ubuntu (e.g. the latest LTS release),
we recommend using the `deadsnakes PPA` to install Python 3.6:

```bash
$ sudo apt-get install software-properties-common
$ sudo add-apt-repository ppa:deadsnakes/ppa
$ sudo apt-get update
$ sudo apt-get install python3.6
```

If you are using other Linux distribution, chances are you already have
Python 3 pre-installed as well.
If not, use your distribution’s package manager.

For example on Fedora, you would use `dnf`:


```bash
$ sudo dnf install python3
```

Note that if the version of the python3 package is not recent enough for you, there may be ways of installing more recent versions as well, depending on you distribution. For example installing the python36 package on Fedora 25 to get Python 3.6. If you are a Fedora user, you might want to read about multiple Python versions available in Fedora.

#### Setuptools & Pip

The two most crucial third-party Python packages are `setuptools` and `pip`.

Once installed, you can download, install and uninstall any compliant
Python software product with a single command.
It also enables you to add this network installation capability to
your own Python software with very little work.

Python 2.7.9 and later (on the python2 series), and Python 3.4 and later
include `pip` by default.

To see if `pip` is installed, open a command prompt and run:

```bash
$ command -v pip
```

To install pip, follow the official pip installation guide -
this will automatically install the latest version of `setuptools`.

Note that on some Linux distributions including Ubuntu and Fedora the `pip`
command is meant for Python 2, while the `pip3` command is meant for Python 3.

```bash
$ command -v pip3
```

Now let's install `jupyter notebook`:

```bash
pip3 install jupyter
```

### Python 3 on macOS

While macOS comes with a large number of UNIX utilities, those familiar with Linux systems will notice one key component missing: a package manager. `Homebrew` fills this lack.

To install `Homebrew`, open Terminal or your favorite OSX terminal emulator and run

```bash
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

The script will explain what changes it will make and prompt you before the installation begins. Once you’ve installed `Homebrew`, insert the `Homebrew` directory at the top of your PATH environment variable. You can do this by adding the following line at the bottom of your `~/.profile` file

```bash
export PATH=/usr/local/bin:/usr/local/sbin:$PATH
```

Now, we can install Python 3:

```bash
$ brew install python
```

This will take a minute or two.

#### `Pip`
`Homebrew` installs `pip` pointing to the Homebrew'd Python 3 for you.

At this point, you have the system Python 2.7 available, potentially the Homebrew version of Python 2 installed, and the Homebrew version of Python 3 as well.

```bash
$ python
```

will launch the homebrew-installed Python 3 interpreter.

```bash
$ python2
```

will launch the homebrew-installed Python 2 interpreter (if any).

```bash
$ python3
```

will launch the homebrew-installed Python 3 interpreter.

If the `Homebrew` version of Python 2 is installed then `pip2` will point to Python 2. If the `Homebrew` version of Python 3 is installed then `pip` will point to Python 3.

Now let's install `jupyter notebook`:

```bash
pip3 install jupyter
```

### Python 3 on Windows


First check whether your computer is running a 32-bit version or a 64-bit version of Windows, by pressing the Windows key + Pause/Break key which will open your System info, and look at the "System type" line. You can download Python for Windows from the website https://www.python.org/downloads/windows/. Click on the "Latest Python 3 Release - Python x.x.x" link. If your computer is running a 64-bit version of Windows, download the Windows x86-64 executable installer. Otherwise, download the Windows x86 executable installer. After downloading the installer, you should run it (double-click on it) and follow the instructions there.

One thing to watch out for: during the installation, you will notice a window marked "Setup". Make sure you tick the "Add Python 3.6 to PATH" checkbox and click on "Install Now", as shown here:

<img src='https://tutorial.djangogirls.org/en/python_installation/images/python-installation-options.png'>

Don't forget to add Python to the Path

In upcoming steps, you'll be using the Windows Command Line (which we'll also tell you about). For now, if you need to type in some commands, go to Start menu → Windows System → Command Prompt. You can also hold in the Windows key and press the "R"-key until the "Run" window pops up. To open the Command Line, type "cmd" and press enter in the "Run" window. (On newer versions of Windows, you might have to search for "Command Prompt" since it's sometimes hidden.)

<img src='https://tutorial.djangogirls.org/en/python_installation/images/windows-plus-r.png'>

Type "cmd" in the "Run" window

Note: if you are using an older version of Windows (7, Vista, or any older version) and the Python 3.6.x installer fails with an error, you can try either:

install all Windows Updates and try to install Python 3.6 again; or
install an older version of Python, e.g., 3.4.6.
If you install an older version of Python, the installation screen may look a bit different than shown above. Make sure you scroll down to see "Add python.exe to Path", then click the button on the left and pick "Will be installed on local hard drive":

<img src='https://tutorial.djangogirls.org/en/python_installation/images/add_python_to_windows_path.png'>

Now let's install `jupyter notebook`:

```
C:\Users\Name\> pip3 install jupyter`
```

# Notebook Format

If you don't know what a Jupyter notebook is, or how to use it, please take a look at this quick
introductory tour: [IPython Notebook Beginner Guide](http://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/index.html).

For additional details and materials on Jupyter and IPython, I suggest this
[Jupyter Notebook the Definitive Guide](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook):

- [What is a Jupyter Notebook](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook#WhatIs)
- [Practical Introduction](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook##UseJupyter)
- [Notebook Examples](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook##NotebookExamples)

If you jumped to this section, skipping the installation step,
please go back to the <a href="#installation">installation guide<a/>
section.
