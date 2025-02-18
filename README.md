# datafun-06-eda

## Purpose
The purpose of Project 6 is to create our own explortatory data analysis but using our own dataset to explore data analysis tools like pandas, seaborn, matpotlib using Jupyter. The dataset that will be analyzed in this project is a seaborn dataset about exercise. 
https://github.com/mwaskom/seaborn-data/blob/master/exercise.csv

# Setting up Project 6

## Make repository in Github and clone to local workspace
```bash
git clone https://github.com/egbogbo11/datafun-06-eda 
```

## Create .gitignore file
Ensure the following entries are added to your .gitignore file to exclude unnecessary files from being committed:

```bash
# Python virtual environment
.venv/

# Visual Studio Code settings and workspace
.vscode/

# Compiled Python files
__pycache__/

# macOS system files
.DS_Store

# Editor backup files
*~

# Python Jupyter Notebook checkpoints and runtime files
.ipynb_checkpoints/
*.ipynb_meta/

## Create and activate virtual environment

Create a virtual environment:

```bash
python -m venv .venv
```

Activate the virtual environment:

```bash
.\.venv\Scripts\activate
```
## Create requirement.txt and download imports
Add the following libraries to your requirements.txt file:

```bash
jupyterlab
numpy
pandas
pyarrow
matplotlib
seaborn
```
Install into your active project virtual environment with this command:

```bash
py -m pip install -r requirements.txt
```
## Stage and Push Files to GitHub

Use the following Git commands to stage and commit changes:

```bash
git status
git add .
git commit -m "commit: message"
git push origin main
```