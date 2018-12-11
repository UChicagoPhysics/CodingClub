---
layout: default
title: Starter Kit
navigation_weight: 2
---

# Starter Kit

Welcome to the [UChicago Physics Coding Club](../) Starter Kit!

This *Starter Kit* provides some tools that will help get you started with coding with `python`, plotting and visualization, and data analysis.

Click [here to go back to the main page](../).

# Programming languages, software, and platforms

## `python`

The [Starter Kit](./) and [Tutorials](../Tutorials/README.md) will primarily use `python`, although any programming language will do. 

`python` which is a powerful, and high-level language that is used across much of academia and industry in one form or another, and so is a very sensible language to use here.

## Installation

The easiest way to get and manage all of these packages is through a package manager such as `conda`; we recommend using Anaconda for this.

* Anaconda: https://www.anaconda.com/

This is easy to use on almost any operating system.

## `python` Software packages

One of the primary sets of packages that we will be using is referred to as the *scipy stack*.

* Scipy: https://www.scipy.org/

The reason for this is that it includes these incredibly powerful, ubiquitous, and useful packages:

* `numpy`: http://www.numpy.org/
   * arrays and mathematics
* `matplotlib`: https://matplotlib.org/
   * plotting
* `IPython`/`Jupyter`: http://ipython.org/
   * notebook interface for python
* `pandas`: http://pandas.pydata.org/
   * dataframes and structures

## Jupyter notebooks

One of the easiest to use applications for python-based computational physics is Jupyter Notebooks.

* `Jupyter`: http://jupyter.org/

These are interactive, easy-to-use interfaces that make writing simple and moderately complex software programs enjoyable and straightforward. The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.

# Version control

## Git, GitHub

`git` is a version-control system that allows you to track changes in your code and facilitate collaboration with others.
`git` is used throughout the science and programming communities and can be an invaluable tool when working on coding projects.

* `git`: https://git-scm.com/

Most people interact with `git` using GitHub (that's this thing you're using now on the web):

* GitHub: https://github.com/

Graphical user interface (GUI) applications are also available for `git`:

* GitKraken: https://www.gitkraken.com/
* Sublime Merge: https://www.sublimemerge.com/

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

* https://guides.github.com/activities/hello-world/
* https://guides.github.com/introduction/flow
* https://guides.github.com/activities/forking/


# Other useful information

### Slack channels

A dedicated Slack discussion channel is available for real-time discussions, sharing of code and results, and other communications.

Sign-up at:
* [uchicagocodingclub.slack.com](https://uchicagocodingclub.slack.com)


### Text editors

A common way to program is through text editors or integraded development environments (IDEs).

There are many good text editors that work on most systems:

* Atom: https://atom.io/
* Visual Studio Code: [https://code.visualstudio.com/
* Sublime Text: https://www.sublimetext.com/

These text editors can run python source code (`.py`) files, but won't be able to work with Jupyter Notebooks, so we recommend that you only use them if you feel more comfortable with programming outside of the notebook interface.



Click [here to go back to the main page](./).
