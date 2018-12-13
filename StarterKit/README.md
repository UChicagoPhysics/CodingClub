---
layout: default
title: Starter Kit
nav_order: 2
navigation_weight: 2
---

# Starter Kit
{: .no_toc }

Welcome to the [UChicago Physics Coding Club](../) Starter Kit!

This *Starter Kit* provides some tools that will help get you started with coding with `python`, plotting and visualization, and data analysis.

Click [here to go back to the main page](../).

---

### Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

# Programming languages, software, and platforms

## `python`

The [Starter Kit](./) and [Tutorials](../Tutorials/README.md) will primarily use `python`, although any programming language will do. 

`python` which is a powerful, and high-level language that is used across much of academia and industry in one form or another, and so is a very sensible language to use here.

## Installation

The easiest way to get and manage all of these packages is through a package manager such as `conda`; we recommend using Anaconda for this.

* Anaconda: [www.anaconda.com/](https://www.anaconda.com)

This is easy to use on almost any operating system.
Note: `conda` is available through both Anaconda and Miniconda; while both work, we will assume Anaconda throughout as that comes with all of the packages we will use and doesn't require the use of the command line interface (CLI).

### macOS

More detailed installation information [here](https://conda.io/docs/user-guide/install/macos.html).

Apple provides most tools you would want through `terminal.app`, found in the `~/Applications/Utilities/` folder.
While you don't need to do use the CLI for most tasks, it offers a significant amount of power and flexibility and so can be valuable to learn.

Once you've installed Anaconda, you should be able to open up a terminal and type:
`conda --version`
to verify that `conda` has been successfully installed and is usable on your machine.

### Windows

More detailed installation information [here](https://conda.io/docs/user-guide/install/windows.html).

Microsoft's prebundled CLI, `Cmd.exe`, lacks some important features that we will want for programming, so we recommend installing another terminal emulator.
We suggest doing a full download of [Cmder](http://cmder.net/); there is also Microsoft's [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/about) for those more familiar with Linux.

During installation of Anaconda, you will be prompted on whether or not you want to add Anaconda to your PATH environment variable.
While Anaconda does not recommend this, if you have not used `python` before then you should not run into any problems, and you may later wish that you _had_ put Anaconda in your PATH (this can be done manually whenever you wish as well).
Hence, provided you don't have another installation of python on your machine, it will not hurt to add Anaconda to your path now, but you do not need to do so unless you are interested in working with the CLI.

Once Anaconda has been installed, you should be able to run it from the *Start* menu by opening the Anaconda prompt.

### Linux

More detailed installation information [here](https://conda.io/docs/user-guide/install/linux.html).

As with macOS, most (if not all) Linux distributions come prepackaged with fully usable terminal emulators and should be usable out of the box.

Once you've installed Anaconda, you should be able to open up a terminal and type:
```conda --version```
to verify that `conda` has been successfully installed and is usable on your machine.

### Chrome OS

Google's Chromebook operating system now (for versions 53 or newer) [supports Android apps](https://support.google.com/googleplay/answer/7021273?hl=en), which give more flexibility in terms of programming and development.

In particular, [Termux](https://termux.com/) gives you access to a fantastic termunal emulator similar to what you would find in a more traditional Unix (Linux, macOS, etc...) desktop environment.
While Termux can get most, if not all, of the work we want done, the lack of a graphical user interface (GUI) means that `Jupyter` notebooks aren't an option here.
Furthermore, there is no easy installation of `conda` here either, so you will need to install most packages manually.
Consequently, unless you are already familiar and comfortable with the CLI, you may want to look to the following section.

### Browser

Depending on your operating system and hardware, the above options might not be viable for you, so there are some browser-based alternatives that should get you up-and-running quickly and easily.
If you don't want to install more software on your computer then this is also a good option; note that this method will not require the Anaconda installation.

Google's [Coloboratory](http://colab.research.google.com/) is a fantastic option and well-suited for our purposes here as it comes with `Jupyter` and all of the packages we're interested in using.

## `python` Software packages

One of the primary sets of packages that we will be using is referred to as the *scipy stack*.

* Scipy: [www.scipy.org](https://www.scipy.org/)

The reason for this is that it includes these incredibly powerful, ubiquitous, and useful packages:

* `numpy`: [www.numpy.org](http://www.numpy.org/)
   * arrays and mathematics
* `matplotlib`: [matplotlib.org](https://matplotlib.org/)
   * plotting
* `IPython`/`Jupyter`: [ipython.org](http://ipython.org/)
   * notebook interface for python
* `pandas`: [pandas.pydata.org](http://pandas.pydata.org/)
   * dataframes and structures

All of these packages are installed _by default_ with `Anaconda`, so you shouldn't need to worry about getting these individually.

## Jupyter notebooks

One of the easiest to use applications for python-based computational physics is Jupyter Notebooks.

* `Jupyter`: [jupyter.org](http://jupyter.org/)

These are interactive, easy-to-use interfaces that make writing simple and moderately complex software programs enjoyable and straightforward. The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.

To run a `Jupyter` notebook, one simply needs to open a terminal and execute the following command:
```jupyter notebook```
which should begin a `jupyter` notebook session in your default browser.
If you are running Windows, you should also be able to click the `Jupyter Notebook` icon installed by Anaconda in the start menu.

# Version control

## Git, GitHub

`git` is a version-control system that allows you to track changes in your code and facilitate collaboration with others.
`git` is used throughout the science and programming communities and can be an invaluable tool when working on coding projects.

* `git`: [git-scm.com](https://git-scm.com/)

Most people interact with `git` using GitHub (that's this thing you're using now on the web):

* GitHub: [github.com](https://github.com/)

Graphical user interface (GUI) applications are also available for `git`:

* GitKraken: [www.gitkraken.com](https://www.gitkraken.com/)
* Sublime Merge: [sublimemerge.com](https://www.sublimemerge.com/)

For those familiar and comfortable with the command line, `git` can also be used directly from a terminal.

## Example

You are not only welcome, but *encouraged* to "fork" this repository directly to your own respository and develop it further

To do this:

1. Fork this repository by clicking on the "Fork" button above
1. Clone your fork of the repository to your computer (find repository in your GitHub user profile, and clone it from there)

If there are updates to this repository that you want to get:

1. Check if your repository is in a clean state with `git status`
1. If it is not, you will need to clean it up (more info below)
1. If it is, then make sure you are on your `master` branch with `git branch`

If you aren't in a clean state, you need to check it out with `git checkout master`
Now you are ready to update:
```
git fetch
git merge
```

Now you should have the up-to-date repository.

1. On your computer you should make a new branch if you want to play aroud
```
git branch play
git checkout play
```
now you can make changes without conflicting with the `master` branch.
To save your changes

There are a huge number of `git` and `GitHub` tutorials out there, but here are a few good ones:

* [guides.github.com/activities/hello-world](https://guides.github.com/activities/hello-world/)
* [guides.github.com/introduction/flow](https://guides.github.com/introduction/flow)
* [guides.github.com/activities/forking](https://guides.github.com/activities/forking/)


# Other useful information

### Slack channels

A dedicated Slack discussion channel is available for real-time discussions, sharing of code and results, and other communications.

Sign-up at:
* [uchicagocodingclub.slack.com](https://uchicagocodingclub.slack.com)

Once you've registered on the Slack workspace, feel free to ask questions in any of the channels or to send direct messages.
Remember, don't hesitate to ask for help!

### Text editors

A common way to program is through text editors or integraded development environments (IDEs).

There are many good text editors that work on most systems:

* Atom: [atom.io](https://atom.io/)
* Visual Studio Code: [code.visualstudio.com](https://code.visualstudio.com/)
* Sublime Text: [www.sublimetext.com](https://www.sublimetext.com/)

These text editors can edit and run python source code (`.py`) files, but won't be able to work with Jupyter Notebooks, so we recommend that you only use them if you feel more comfortable with programming outside of the notebook interface.



Click [here to go back to the main page](./).
