
# PyCon Nove Beginner's Day
Before using the notebooks please install `Python` and `virtualenv` according to your operating system.

# Installation Guides
These guides go over the proper installation of Python for development purposes, as well as `setuptools`, `pip` and `virtualenv`.

## Python 3 Installation Guides

### Python 3 on Linux

To see which version of Python 3 you have installed, open a command prompt and run:

```bash
$ python3 --version
```

If you are using Ubuntu 16.10 or newer, then you can easily install Python 3.6 with the following commands:

```bash
$ sudo apt-get update
$ sudo apt-get install python3.6
```

If you’re using another version of Ubuntu (e.g. the latest LTS release), we recommend using the `deadsnakes PPA` to install Python 3.6:

```bash
$ sudo apt-get install software-properties-common
$ sudo add-apt-repository ppa:deadsnakes/ppa
$ sudo apt-get update
$ sudo apt-get install python3.6
```

If you are using other Linux distribution, chances are you already have Python 3 pre-installed as well. If not, use your distribution’s package manager. For example on Fedora, you would use `dnf`:


```bash
$ sudo dnf install python3
```

Note that if the version of the python3 package is not recent enough for you, there may be ways of installing more recent versions as well, depending on you distribution. For example installing the python36 package on Fedora 25 to get Python 3.6. If you are a Fedora user, you might want to read about multiple Python versions available in Fedora.

#### Setuptools & Pip

The two most crucial third-party Python packages are `setuptools` and `pip`.

Once installed, you can download, install and uninstall any compliant Python software product with a single command. It also enables you to add this network installation capability to your own Python software with very little work.

Python 2.7.9 and later (on the python2 series), and Python 3.4 and later include `pip` by default.

To see if `pip` is installed, open a command prompt and run:

```bash
$ command -v pip
```

To install pip, follow the official pip installation guide - this will automatically install the latest version of `setuptools`.

Note that on some Linux distributions including Ubuntu and Fedora the `pip` command is meant for Python 2, while the `pip3` command is meant for Python 3.

```bash
$ command -v pip3
```

However, when using virtual environments (described below), you don’t need to care about that.

#### Virtual Environments
The next step is to install `virtualenv` so you can install dependencies and manage virtual environments.

A Virtual Environment is a tool to keep the dependencies required by different projects in separate places, by creating virtual Python environments for them. It solves the “Project X depends on version 1.x, but Project Y needs 4.x” dilemma, and keeps your global site-packages directory clean and manageable.

For example, you can work on a project which requires Django 1.10 while also maintaining a project which requires Django 1.8.

`virtualenv` is a tool to create isolated Python environments. `virtualenv`: creates a folder which contains all the necessary executables to use the packages that a Python project would need.

**Installing `virtualenv` via `pip`**:

```bash
$ pip install virtualenv
```

**Test your installation:**

```bash
$ virtualenv --version
```

**Create a virtual environment for a project:**

```bash
$ cd my_project_folder
$ virtualenv my_project
```

`virtualenv` my_project will create a folder in the current directory which will contain the Python executable files, and a copy of the `pip` library which you can use to install other packages. The name of the virtual environment (in this case, it was `my_project`) can be anything you want; omitting the name will place the files in the current directory instead.

This creates a copy of Python in whichever directory you ran the command in, placing it in a folder named `my_project`.

**To activate the `virtualenv`:**

```bash
$ source my_project/bin/activate
```

**To deactivate:**

```bash
$ deactivate
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

#### Virtual Environments
The next step is to install `Virtualenv`, so you can install dependencies and manage virtual environments.

A Virtual Environment is a tool to keep the dependencies required by different projects in separate places, by creating virtual Python environments for them. It solves the “Project X depends on version 1.x but, Project Y needs 4.x” dilemma, and keeps your global site-packages directory clean and manageable.

For example, you can work on a project which requires Django 1.10 while also maintaining a project which requires Django 1.8.

`virtualenv` is a tool to create isolated Python environments. `virtualenv` creates a folder which contains all the necessary executables to use the packages that a Python project would need.

**Install `virtualenv` via `pip`**:

```bash
$ pip install virtualenv
```

**Test your installation:**

```bash
$ virtualenv --version
```

**Create a virtual environment for a project:**

```bash
$ cd my_project_folder
$ virtualenv my_project
```

`virtualenv my_project` will create a folder in the current directory which will contain the Python executable files, and a copy of the `pip` library which you can use to install other packages. The name of the virtual environment (in this case, it was `my_project`) can be anything you want; omitting the name will place the files in the current directory instead.

This creates a copy of Python in whichever directory you ran the command in, placing it in a folder named `my_project`.

**To activate the `virtualenv`:**

```bash
$ source my_project/bin/activate
```

**To deactivate:**

```
$ deactivate
```

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

#### Virtual environment
Before installing software via `pip` we will get you to install an extremely useful tool to help keep your coding environment tidy on your computer. It's possible to skip this step, but it's highly recommended. Starting with the best possible setup will save you a lot of trouble in the future!

So, let's create a virtual environment (also called a virtualenv). `virtualenv` will isolate your Python setup on a per-project basis.

All you need to do is find a directory in which you want to create the virtualenv; your home directory, for example. On Windows, it might look like 

```
C:\Users\Name\ (where Name is the name of your login).
```

NOTE: On Windows, make sure that this directory does not contain accented or special characters; if your username contains accented characters, use a different directory, for example, `C:\myproject`.

To create a new virtualenv, you need to open the command prompt and run 

```
python -m venv myvenv
```

where `myvenv` is the name of your virtualenv. You can use any other name, but stick to lowercase and use no spaces, accents or special characters. It is also good idea to keep the name short – you'll be referencing it a lot!

The command above will create a directory called `myvenv` (or whatever name you chose) that contains our virtual environment (basically a bunch of directory and files).

Start your virtual environment by running:

```
C:\Users\Name\> myvenv\Scripts\activate
```

Now let's install `jupyter notebook`:

```
C:\Users\Name\> pip3 install jupyter`
```
