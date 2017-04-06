# LARICS Introduction to Git Tutorial

Presentation for the git intro tutorial.

## Building the document ##

The main document (the one you should run `pdflatex` on) is `larics-git-tutorial-intro.tex`. The LaTeX code uses the [minted](https://www.ctan.org/pkg/minted) package, so it is necessary to add the `-shell-escape` option to the pdflatex command line when compiling the document.

## Notes to lecturers ##

The classes are interactive, i.e., students are expected to follow along on their own laptops.

The material is appropriate for 2 classes of 2 hours (2x105 minutes). The first class should cover material up to the "Branches in git" slide. The second class should cover the material on working with branches.

The students should arrive to class prepared, i.e., they should:

- [Open a GitHub account](https://github.com/join?source=header-home)
- [Check for existing ssh keys](https://help.github.com/articles/checking-for-existing-ssh-keys/)
- In case they do not have a key, they should [generate a new ssh key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)
- [Add the key to their GitHub account](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)

To check that the key was successfully added they should try logging on to git (answer yes if prompted):
```
$ sudo ssh git@github.com
Hi <user>! You've successfully authenticated, but GitHub does not provide shell access.
Connection to github.com closed.
```
On Linux, the following software must be installed:
```
$ sudo apt-get install git git-gui gitg
```

Optionally, students who whish to work on the C++ example should also install:
```
$ sudo apt-get install build-essential cmake
```

The classes can also be followed on Windows, with the help of the following software:

  - [Git for Windows](https://git-for-windows.github.io/)
  - [The gitg Windows client](https://git-scm.com/download/gui/windows) (path to the executable must be added to the Windows PATH environment variable)
  - [mingw](http://www.mingw.org/) and [CMake](https://cmake.org/download/) or [Python](https://www.python.org/downloads/windows/) (theoretically, but the demo code currently seems to break on Windows)

