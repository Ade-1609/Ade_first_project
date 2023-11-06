Exploratory Data Analysis
## Description
This exploratory data analysis seeks to make recommendations to my clients on the best time to list his apartments for sale, and advise of renovation decisions .
- House sales in King County 2014 - 2015
## Hypothesis
Null: Renovation = 0 impact on selling price. 
Alternate: Renovation has an impact on selling price.
## Methodology
The use of bar plots, line plot and geographical plot will be used to prove of disprove the null hypothesis.

## Summary
Our finding shows, we have to reject our null hypothesis which says renovation would have no impact on selling price and accept the alternate hypothesis.
There is a positive relationship between renovation and selling price. 
Renovated apartments are likely to sell at a higher price on average when compared to non renovated apartments.
Accounting for factors including waterfront and grade, result largely holds true
This finding holds for other houses not in clients portfolio( 2,4,5).
Positive association noticed does not imply causality.


## Recommendations
In most cases, apartment will likely lead to a big return but it will be important to consider the cost of renovation.
For apartments that fall under  grade 3, renovating before sale would be the better outcome .
For apartments in grade 2, if cost of renovation below X, proceed with renovation.
For apartments in grade 1, do not renovate. 
After renovating, the apartment should be sold in December, best period to maximise earning potential.


# Setup

One of the first steps when starting any data science project is to create a virtual environment. For this project you have to create this environment from scratch yourself. However, you should be already familiar with the commands you will need to do so. The general workflow consists of... 

* setting the python version locally to 3.11.3
* creating a virtual environment using the `venv` module
* activating your newly created environment 
* upgrading `pip` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
* installing the required packages via `pip`

At the end, you want to make sure that people who are interested in your project can create an identical environment on their own computer in order to be able to run your code without running into errors. Therefore you can create a `requirements file` and add it to your repository. You can create such a file by running the following command: 

```bash
pip freeze > requirements.txt
```

### Environment

This repo contains a requirements.txt file with a list of all the packages and dependencies you will need. Before you install the virtual environment, make sure to install postgresql if you haven't done it before.

```bash
brew update
brew install postgresql@14
```

In order to install the environment you can use the following commands:

```
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```