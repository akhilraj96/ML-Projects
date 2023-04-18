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

```
MLProjects
│   .gitignore
│   README.md
│   requirements.txt
│   setup.py
│
└───src
│   │   __init__.py
│   │   exception.py
│   │   logger.py
│   │   utils.py
│   │
│   └───components
│   │   │   __init__.py
│   │   │   data_ingestion.py
│   │   │   data_transformation.py
│   │   │   model_trainer.py
│   │
│   └───pipeline
│       │   __init__.py
│       │   predict_pipeline.py
│       │   train_pipeline.py
│
└───env
│
└───logs
│
└───MLProjects.egg-info

```

- setup.py

  The setup script is the centre of all activity in bulding, distributing and installing required modules.

  In the script an external file(requirements.txt) is used to install the requirements for the project.

- requirements.txt

  This is a file listing all the dependencies of the project.

- src\

  This folder contains all the source files of the project.

  - exception.py

    To create a custom exception

  - logger.py

    To create a logging template
