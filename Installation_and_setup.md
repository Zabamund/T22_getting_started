# Installation and Setup

<!-- .slide: data-background="./images/Agile_logo.png" -->

---

## Getting python installed on your computer

----

### python.org

![Install from python.org](./images/install_from_python_org.png)

Note: Navigate to python.org, select the Download option, and then choose the option that's right for your Operating System (OS)

----

### Miniconda

> Miniconda is a free minimal installer for conda. It [...] includes only conda, Python, the packages they depend on, and a small number of other useful packages [...].

1. Click the 64-bit Python 3.9 version download link.
2. Run the installer, accepting the license.
3. Accept the defaults.

[Miniconda Installer Links](https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links)

Note: [Anaconda or miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html#anaconda-or-miniconda)

Choose Anaconda if you:
- Are new to conda or Python.
- Like the convenience of having Python and over 1,500 scientific packages automatically installed at once.
- Have the time and disk space---a few minutes and 3 GB.
- Do not want to individually install each of the packages you want to use.
- Wish to use a set of packages curated and vetted for interoperability and usability.

Choose Miniconda if you:
- Do not mind installing each of the packages you want to use individually.
- Do not have time or disk space to install over 1,500 packages at once.
- Want fast access to Python and the conda commands and you wish to sort out the other programs later.

----

### Anaconda

> Your data science toolkit
[...] the open-source Individual Edition (Distribution) is the easiest way to perform Python/R data science and machine learning on a single machine.

[Anaconda Individual Edition](https://www.anaconda.com/products/individual)

Note: For enterprise editions, see [pricing](https://www.anaconda.com/pricing)

----

### A Note on different operating systems

Python is **platform independant**, you can install it on Windows, Mac or GNU/Linux. There are even versions of python for [other platforms](https://www.python.org/download/other/).

---

## Creating a coding environment

Writing code is an exercise in dependency management, and ideally, you want to *delegate* that task to an environment manager. That is, a program that will check through all the installed packages (tools) you've installed and make sure all the versions are compatible.

----

### conda, pyenv, virtualenv

We'll use [`conda`](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) in this tutorial but [here](https://stackoverflow.com/questions/38217545/what-is-the-difference-between-pyenv-virtualenv-anaconda) is a nice stack**overflow** discussion of the options at your disposal.

----

### Setting up an environment (1/2)

1. Click on this link and leave the file in your Downloads folder: 
[UPDATE THIS link: T22_getting_started/environment.yml](https://github.com/Zabamund/T22_getting_started/environment.yml)

2. Open an Anaconda Prompt from the Start menu, and type the following (all one line!):

`conda env create -f %USERPROFILE%/Downloads/environment.yml`

Note: For Mac and Linux users, simply save the `environment.yml` file in your Downloads folder, navigate to that folder in your terminal emulator and run `conda env create` (it will us `environment.yml` by default)

----

### Setting up an environment (2/2)

3. Hit return if it asks for confirmation. When finished, start the environment:

`conda activate geocomp`

4. Now one more step to get access to this environment from inside Jupyter (all one line again!): 

`python -m ipykernel install --user --name geocomp`

----

### jupyter

To start coding, run:

`jupyter notebook`

This will start a server and launch the notebook in your default browser:

![the jupyter server](./images/jupyter_server.png)

Note: Simply show whichever notebook instance I have running during demo.

----

### Basic geoscience tool set

Let's open

`environment.yml`

to see what we installed.

Note: Open `./environment.yml` inside the jupyter notebook.

---

## Choosing a text editor

----

### Jupyter

----

### VSCode, Atom, Sublime Text

----

### vi, vim, nano, emacs

---

## Running python from the command line

----

### What is the command line?

----

### When to run python from the CLI

----

### How to run python from the CLI

----

#### Simple code editor

----

#### Powerful script runner

---

## Running python from jupyter notebook

---

## Jupyter notebook, lab, text editors


---

# NEXT: intro to python notebook!