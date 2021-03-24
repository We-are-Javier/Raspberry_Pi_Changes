## Setting up Virtual Environment Wrapper

### Setup:

1. Create a directory to hold the virtual environments.(mkdir $HOME/.virtualenvs).
2. Add a line like `export WORKON_HOME=$HOME/.virtualenvs` to your .bashrc.
3. Add a line like `source /path/to/this/file/virtualenvwrapper.sh` to your .bashrc.
4. Run: source `~/.bashrc`
5. Run: `workon`
6. A list of environments, empty, is printed.
7. Run: `mkvirtualenv temp`
8. Run: `workon`
9. This time, the "temp" environment is included.
10. Run: `workon temp`
11. The virtual environment is activated.

There is a lot more to be done using this wrapper. This guide will not direct you on how to do what I did. Instead, [here is a linke](https://virtualenvwrapper.readthedocs.io/en/latest/install.html) to use if this is something you see as useful.
