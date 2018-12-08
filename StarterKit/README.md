# StarterKit

Welcome to the UChicago Physics CodingClub StarterKit!

This StarterKit provides some tools that will help get you started with coding with python, plotting and visualization, and data analysis.

Click [here to go back to the main page](../).

## Programming Languages, Software, and Platforms

We will primarily be using Python, which is a powerful, and high-level language that is used across much of academia and industry in one form or another.

### Software

One of the primary "sets" of packages that we will be using is referred to as the "scipy stack".

* https://www.scipy.org/

The reason for this is that it includes these incredibly powerful, ubiquitous, and useful packages:

* `numpy`: http://www.numpy.org/ (arrays and mathematics)
* `matplotlib`: https://matplotlib.org/ (plotting)
* `IPython`/`Jupyter`: http://ipython.org/ (notebook interface for python)
* `pandas`: http://pandas.pydata.org/ (dataframes and structures)

The easiest way to get and manage all of these packages is through a package manager such as `conda`; we recommend using Anaconda for this.

* Anaconda: https://www.anaconda.com/

### Platform

One of the easiest to use applications for python-based computational physics is Jupyter Notebooks.

* `Jupyter`: http://jupyter.org/

These are interactive, easy-to-use interfaces that make writing simple and moderately complex software programs enjoyable and straightforward.
The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.

We also have a platform that provisions (creates, maintains, and hosts) Jupyter Notebook instances on-demand:

* https://ml.maniac.uchicago.edu/

To use this service, you will need an account.

### Text Editors

Another common way to program is through text editors or integraded development environments (IDEs).

There are many good text editors that work on most systems:

* Atom: https://atom.io/
* Visual Studio Code: https://code.visualstudio.com/
* Sublime Text: https://www.sublimetext.com/

These text editors can run python source code (`.py`) files, but won't be able to work with Jupyter Notebooks, so we recommend that you only use them if you feel more comfortable with programming outside of the notebook interface.

### Git, GitHub

`git` is a version-control system that allows you to track changes in your code and facilitate collaboration with others.
`git` is used throughout the science and programming communities and can be an invaluable tool when working on coding projects.

* `git`: https://git-scm.com/

Most people interact with `git` using GitHub (that's this thing you're using now on the web):

* GitHub: https://github.com/

Graphical user interface (GUI) applications are also available for `git`:

* GitKraken: https://www.gitkraken.com/
* Sublime Merge: https://www.sublimemerge.com/

For those familiar and comfortable with the command line, `git` can also be used directly from a terminal.

If you are using the `JupyterLab` platform described above, you should have direct access to the example code included in this repository.
However, you are not only welcome, but *encouraged* to "fork" this repository directly to your own respository and develop it further

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


Click [here to go back to the main page](./).
