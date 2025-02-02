# learn-python3-2025
Spend some time learning advancements in Python and related technologies in 2025

# Clone the git repo in dev box. 
```
kaunjovi@devbook code % git clone git@github.com:kaunjovi/learn-python3-2025.git
Cloning into 'learn-python3-2025'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (4/4), done.
kaunjovi@devbook code % cd learn-python3-2025 
```

# Check for versions 

````
kaunjovi@devbook learn-python3-2025 % where python3
/Library/Frameworks/Python.framework/Versions/3.11/bin/python3
/opt/homebrew/bin/python3
/usr/local/bin/python3
/usr/bin/python3

kaunjovi@devbook learn-python3-2025 % python3 --version 
Python 3.11.9

kaunjovi@devbook learn-python3-2025 % pip --version 
zsh: command not found: pip

kaunjovi@devbook learn-python3-2025 % poetry --version 
Poetry (version 1.8.3)
````

# Enable poetry 
1. Create empty .venv folder 
1. Add .venv to .gitignore file 
1. Use poetry to create the pyproject.toml file. 

```
kaunjovi@devbook learn-python3-2025 % poetry init
```


# Open IDE and start coding. 

```
kaunjovi@devbook learn-python3-2025 % codium .
```


1. https://medium.com/@sjalexandre/python-tutorial-managing-projects-with-poetry-cd2deab72697


# uv 

1. [Installing uv](https://docs.astral.sh/uv/getting-started/installation/)

```
kaunjovi@devbook learn-python3-2025 % curl -LsSf https://astral.sh/uv/install.sh | sh
downloading uv 0.5.26 aarch64-apple-darwin
no checksums to verify
installing to /Users/kaunjovi/.local/bin
  uv
  uvx
everything's installed!
```

1. Check if you have the latest uv 

```
kaunjovi@devbook learn-python3-2025 % uv self update
info: Checking for updates...
success: You're on the latest version of uv (v0.5.26)
```

1. Getting started. Get uv to start talking. 

```
kaunjovi@devbook learn-python3-2025 % uv 
An extremely fast Python package manager.

Usage: uv [OPTIONS] <COMMAND>

Commands:
  run      Run a command or script
  ...
  ...
```

1. Have uv start a python project. 

```
kaunjovi@devbook learn-python3-2025 % uv init
Initialized project `learn-python3-2025`
```

1. Start a virtual environment 

```
kaunjovi@devbook learn-python3-2025 % uv venv 
Using CPython 3.11.9 interpreter at: /Library/Frameworks/Python.framework/Versions/3.11/bin/python3.11
Creating virtual environment at: .venv
Activate with: source .venv/bin/activate
```

1. Start a virtual environment and run the apps 

```
uv sync
source .venv/bin/activate
python example.py
```
