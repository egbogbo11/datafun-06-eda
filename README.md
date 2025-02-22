# datafun-06-eda

## Purpose
The purpose of Project 6 is to create our own explortatory data analysis but using our own dataset to explore data analysis tools like pandas, seaborn, matpotlib using Jupyter. The dataset that will be analyzed in this project is a seaborn dataset about restaurants. 
https://github.com/mwaskom/seaborn-data/blob/master/tips.csv

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

## To complete Project 6: 

Step 1:

Make sure Jupyter is installed and working in your project virtual environment. Document the process and commands you used in your README.md.

Then create, open, and start a new notebook in your root project repository folder:

Create the Notebook: In the VS Code Explorer, create a new file i.e., yourname_eda.ipynb. Ensure it has a .ipynb extension.
Verify your new notebook is open for editing. If needed, view the project files in VS Code Explorer and double-click the notebook file to open it for editing.
Add a Markdown cell at the top of your notebook with the introduction (include the title, author, date and the purpose of the project).

Step 2: 

Add a Python cell next with the import statements for the libraries you will use in the project. Follow conventional package import organization and alias. Import each package just once near the top of the file. Be sure you have INSTALLED any external packages (outside the Python Standard Library) into your active project virtual environment first.

Step 3: 

Perform a unique exploratory data analysis project using the tools and skills covered previously.
```bash
Step 1. Data Acquisition

Load the data into a pandas DataFrame. Use the pd read functions such as pd.read_csv() or pd.read_excel() as appropriate. To read from the Seaborn dataset, we'll use sns.load_dataset() function and pass in the 'iris' (the name without .csv) to populate our DataFrame.

Step 2. Initial Data Inspection

Display the first 10 rows of the DataFrame, check the shape, and display the data types of each column using df.head(10), df.shape, and df.dtypes.

Step 3. Initial Descriptive Statistics

Use the DataFrame describe() method to display summary statistics for each column.

Step 4. Initial Data Distribution for Numerical Columns

Choose a numerical column and use df['column_name'].hist() to plot a histogram for that specific column. To show all the histograms for all numerical columns, use df.hist(). Afterwards, use a Markdown cell to document your observations.

Step 5. Initial Data Distribution for Categorical Columns

Choose a categorical column and use df['column_name'].value_counts() to display the count of each category. Use a loop to show the value counts for all categorical columns. Afterwards, use a Markdown cell to document your observations.

Step 6. Initial Data Transformation and Feature Engineering

Use pandas and other tools to perform transformations. Transformation may include renaming columns, adding new columns, or transforming existing data for more in-depth analysis.

For this project, you must:

Rename at least one column. Add at least one column.

Step 7. Initial Visualizations

Create a variety of chart types using seaborn and matplotlib to showcase different aspects of your data. For each chart, include the goal - what you want to learn/explore, the type of chart you choose, display the chart, and tell your data story. Use Markdown cells and Python cells. Create at least 3 subsections - each subsection should have the following parts:

Goal: The question you are exploring.

Chart Type: Tell us what kind of chart you choose to illustrate this goal.

Chart: Display the chart.

Story: Use Markdown cell(s) to document your observations and insights.

Step 8. Initial Storytelling and Presentation

Present your notebook with an opening that introduces yourself and your topic. Use Markdown section headings to introduce each step. Interpret the visualizations and statistics to narrate a clear and compelling data story. Present your findings in a logical and engaging manner.
```