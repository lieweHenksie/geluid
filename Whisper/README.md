# Whisper, install.

This is a first version build.  
Please see the [reading-material](#reading-material) for more in-depth explanations.  

## Setting up and activating the .venv
To create a virtual environment, run:  

### Windows:
`c:\>python -m venv .venv --copies`
### Ubuntu:
`python3 -m venv .venv --copies`

If you want to, you can set your bash context so that all Python commands run in the virtual environment, by running:

`source .venv/bin/activate`

to deactivate a virtual environment, run:
`deactivate`

## Installing the Required Python Modules (pipenv)
Install pipenv package for easier package management

### Windows:
`pip install pipenv`
### Ubuntu:
`pip install pipenv`

Now use pipenv to install the production modules, by running 

### Windows:
`pipenv install`
### Ubuntu:
`pipenv install`

or install the entire dev stack by typing 

### Windows:
`pipenv install --dev`
### Ubuntu:
`pipenv install --dev`

## Configuration
You need to place a `.env` file in your `src` folder for configuring different environments.  
You can copy and rename the `.env.example` file to know which ones are necessary/available.  

### Ubuntu:
`cp .env.example .env`  

## Running the main script
From within the virtual environment point first to the python compiler, then to the main.py script. 

For me this would be 
### Ubuntu:
`python src/main.py`

### Windows:
`python src\main.py`

## Building for staging & production
### Windows:
`.\scripts\package.cmd`
### Ubuntu:
`./scripts/package.sh`

### reading material:
- https://openai.com/blog/whisper/
