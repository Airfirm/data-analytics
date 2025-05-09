"""
This contains reusable tools for Data Analytics Fundamental Projects, it consist of Analytics about a firm Byline

File: utils_oluwafemi.py

Purpose: Reusable Module for My Analytics Projects

Description: This module provides a byline for my analytics projects. 
When we work hard to write useful code, we want it to be reusable.
A good byline could be used in every Python analytics project we do.

Author: Oluwafemi Salawu

Date: 2025-05-09
Copyright (c) 2023 Oluwafemi Salawu
"""

#####################################
# Import Modules
#####################################

# Import helpful modules from the Python Standard library
# See more at: https://docs.python.org/3/library/

import statistics


#####################################
# Declare Global Variables
#####################################

# declare a boolean variable (has a value True or False)
# TODO: Add another or replace this with your own boolean variable
had_international_clients: bool = False

# declare an integer variable 
# TODO: Add or replace this with your own integer variable
years_in_operation: int = 7

# declare a floating point variable
# TODO: Add or replace this with your own floating point variable
average_client_satisfaction: float = 5.6

# declare a list of strings
# TODO: Add or replace this with your own list  
skills_required: list = ["Data Analytics Engineer", "BI Developer", "Business Technology Product Manager"]

# declare a list of numbers so we can illustrate statistics skills
# TODO: Add or replace this with your own numeric list  
client_satisfaction_scores: list = [45.5, 54.2, 25.1, 16.9, 70.3]

# Calculate basic statistics using built-in Python functions and the statistics module
# TODO: Replace these variable names with the variable name of your own numeric list
minimum_score: float = min(client_satisfaction_scores)  
maximum_score: float = max(client_satisfaction_scores)  
the_mean_score: float = statistics.mean(client_satisfaction_scores)  
standard_deviation_score: float = statistics.stdev(client_satisfaction_scores)

# Use a Python formatted string (f-string) to show information
# TODO: Modify the text in the byline to fit your information
# TODO: Modify the variables in the byline to use your variable names
byline: str = f"""
---------------------------------------------------------
Data Analytics: Delivering Professional Insights To Foster Decison-Making
---------------------------------------------------------
Ever Had An International Clients:  {had_international_clients}
Number Of Years in Operation:         {years_in_operation}
Skills Required:             {skills_required}
Satisfaction Scores: {client_satisfaction_scores}
Lowest Satisfaction Score: {minimum_score}
Highest Satisfaction Score: {maximum_score}
Mean Score: {the_mean_score:.2f}
Standard Deviation Scores: {standard_deviation_score:.2f}
"""

#####################################
# Define global functions
#####################################

def get_byline() -> str:
    '''
    Get a byline for my analytics projects.
       
    Returns a string byline that illustrates my specific skills.

    A function is a block of code that performs a task.
    This function just returns our byline.
    We can call this (or other functions) in later modules 
    so we can write it once and reuse it. 
    We use a type hint to indicate this function returns a string
    (that is, it has a Python type of str).
    It doesn't need any additional information passed in, 
    so there's nothing needed inside the parentheses.
    Everything after the colon must be indented consistently (usually 4 spaces)
    '''
    return byline

#####################################
# Define main function for this module.
#####################################

def main() -> None:
    '''
    Print results of get_byline() when main() is called.

    This function just prints the byline to the console when we run this as a script.
    The type hint indicates this function doesn't return anything when called 
    (that is, it has a Python type of None).
    It doesn't need any additional information passed in, 
    so there's nothing inside the parentheses.
    Everything after the colon must be indented consistently (usually 4 spaces)
    '''

    print("START main() in utils_oluwafemi.py")
    print(get_byline())
    print("END main() in utils_oluwafemi.py")

#####################################
# Conditional Execution
#####################################

# If we are running this file as a script then call main()
# and verify our code works as expected.

if __name__ == '__main__':
    main()


# Pro Analytics 01: Setup and Workflow Guide

This repository provides a clear, concise guide to help set up a machine for Python projects, 
initialize a new Python project, and follow a repeatable project workflow 
when developing professional Python projects. 

The instructions are divided into three main sections.

## First: Set Up Machine & Sign up for GitHub
Go to [01-machine-setup](01-machine-setup/MACHINE-SETUP.md) to prepare for Python projects.
Start here to set up a machine for the first time (or to upgrade or verify professional tools).

This section contains **one-time tasks** including:
1. View file extensions and hidden files and folders.
2. Optional: Install (or verify) a package manager for your operating system.
3. Install Python, Git, and Visual Studio (VS) Code for your operating system.
4. Configure Git
5. Install common VS Code extensions.
6. Create a folder on your machine to hold your GitHub projects. 
7. Create a GitHub account (join 100 Million Developers!)

---

## Second: Initialize a Project
Go to [02-Project-Initialization](./02-project-initialization/PROJECT-INITIALIZATION.md) when **starting a new project**.

This section walks you through the steps to either:
1. Copy an existing project OR start a new project from scratch.
2. Clone your new GitHub repo to your machine. 
3. Add common files such as .gitignore and requirements.txt.
4. Git add-commit-push the changes to GitHub.
5. Create a local project virtual environment for Python.

---

## Third: Work on the Project Over Time
Go to [03-Repeatable-Workflow](./03-repeatable-workflow/REPEATABLE-WORKFLOW.md) for ongoing project development.

This section provides the **repeatable steps** for working on Python projects. 
These steps are typically followed whenever we make changes to a project. The workflow includes:
1. Pull any recent changes from GitHub.
2. Activate the virtual environment.
3. Install dependencies.
4. Run scripts and/or Jupyter notebooks.
5. Make updates, verify the code still runs, and git add-commit-push to GitHub. 

---

## Important

- Follow the instructions carefully.
- Follow the instructions in the recommended order.
- Verify each step before proceeding. 

## Celebrate
Follow each step carefully. 
We have helped hundreds of new analysts get started with professional Python. 
Verify you can run both a script and a notebook successfully. 
Then, celebrate - that's a big iceberg needed to get started with Professional Python.

## Follow The Proven Path Provided
Hopefully, each step is not too bad and things go well. 
When they don't - that's to be expected. 
Part of the reason we get hired is to "figure things out" and we are here to help you do that. 
Learn to do a web search, and experiment with free AI assistants to help explain and provide any additional details needed. 
Remember, YOU are in charge. 
This is the process we support and these instructions work. 
Do NOT deviate unless you agree to invest time and energy to ensure any of the many alternate paths work for you throughout the program. 

## Explore

AFTER that is where the power and joy of working with Python begins. 
Keep good notes. 
Save the working versions and then, change things. For example:

- Rename a variable. 
- Add a new statement. 
- Comment things out.
- Rename a function. 
- View the logs. Log something new (e.g., every function when called and before returning a value).

Working with code is a fun, safe, rewarding way to learn. 
If you enjoy puzzles, getting value from Python is a great way to earn a living. 

## CheatSheet: Commands to Manage Virtual Environment

For Windows PowerShell (change if using Mac/Linux). 
Keep these notes in every project README.md.

```powershell
py -m venv .venv
.\.venv\Scripts\activate
py -m pip install --upgrade pip setuptools wheel
py -m pip install --upgrade -r requirements.txt
```

## CheatSheet: Commands to Run Python Scripts

Remember to activate your .venv (and install packages if they haven't been installed yet) before running files.
Verify that all external packages imported into a file are included in requirements.txt (and have NOT been commented out).

```shell
py demo_script.py
py do_stats.py
py draw_chart.py
py greet_user.py
```

## CheatSheet: Commands to Git add-commit-push

```shell
git add .
git commit -m "custom message"
git push -u origin main
```
