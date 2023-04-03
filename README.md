# ML Projects

## Environment Setup

The first step is to create an environment in side the project repository.

```
conda create -p env python==3.8 -y
conda activate env/
```

Create a .gitignore file to ignore the environment from uploding to github.

```
...
# Environments
.env
.venv
env/                         #environment name
venv/
ENV/
env.bak/
venv.bak/
...
```

## Project Setup

1. setup.py

   The setup script is the centre of all activity in bulding, distributing and installing required modules.

   In the script an external file(requirements.txt) is used to install the requirements for the project.

2. requirements.txt

   This is a file listing all the dependencies of the project.

3. src\

   This folder contains all the source files of the project.
