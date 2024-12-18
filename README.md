# Analysis of the Titanic Dataset

The sinking of the Titanic is one of the most infamous shipwrecks in history.
The following project is an analysis of the Titanic dataset to uncover patterns and insights about the passengers on board. Moreover, it features a logistic regression model to predict survival of passengers onboard.

## Dataset

The primary source of data on Titanic passengers is the Encyclopedia Titanica. The datasets utilized here originated from the efforts of multiple researchers. One notable source is Eaton & Haas's Titanic: Triumph and Tragedy (1994, Patrick Stephens Ltd), which features a passenger list compiled by various researchers and edited by Michael A. Findlay.

The dataset used for this analysis was derived here https://www.kaggle.com/datasets/yasserh/titanic-dataset. 

## Install

In the current Github Repo you may follow the following steps to setup the repo.

```bash
# setup python 3.11 environment
conda create -n py311 python=3.11.10
conda activate py311

# create virtual enviroment for this project
python -m venv .venv


# install packages required by this project
pip install poetry
poetry install
```