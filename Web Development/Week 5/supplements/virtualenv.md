# Web Dev (LS 2020) Supplementary Material: Virtual Environments with *virtualenv*

Python applications will often use packages and modules that don’t come as part of the standard library. Applications will sometimes need a specific version of a library, because the application may require that a particular bug has been fixed or the application may be written using an obsolete version of the library’s interface.

This means it may not be possible for one Python installation to meet the requirements of every application. If application A needs version 1.0 of a particular module but application B needs version 2.0, then the requirements are in conflict and installing either version 1.0 or 2.0 will leave one application unable to run.

The solution for this problem is to create a virtual environment, a self-contained directory tree that contains a Python installation for a particular version of Python, plus a number of additional packages.

## Setting up a Virtual Python environment

There are a number of tools that can be used to create virtual Python enviroments. This tutorial will be covering creating a virtual environment with [__virtualenv__](https://pypi.org/project/virtualenv/).

__via pipx__

virtualenv is a CLI tool that needs a Python interpreter to run. If you already have a Python 3.5+ interpreter the best is to use pipx to install virtualenv into an isolated environment. This has the added benefit that later you’ll be able to upgrade virtualenv without affecting other parts of the system.

`pipx install virtualenv
virtualenv --help`

__via pip__

Alternatively you can install it within the global Python interpreter itself (perhaps as a user package via the --user flag). Be cautious if you are using a python install that is managed by your operating system or another package manager. pip might not coordinate with those tools, and may leave your system in an inconsistent state. Note, if you go down this path you need to ensure pip is new enough per the subsections below:

`python -m pip install --user virtualenv
python -m virtualenv --help`


Here is a [video tutorial](https://youtu.be/N5vscPTWKOk) if the above steps seem overwhelming.


If you face any problems with installation or setup, we are here to resolve them on the [Telegram Group](https://t.me/joinchat/SOmrORRVjQmyIpCeUd-OYw).