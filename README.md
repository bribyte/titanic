# Analysis of the Titanic Dataset

The sinking of the Titanic remains one of history's most notorious maritime disasters. This project delves into the Titanic dataset to uncover patterns and insights about the passengers onboard, while also featuring a logistic regression model to predict passenger survival.

## Exploratory Data Analysis (EDA)

The Exploratory Data Analysis provides a detailed examination of the factors that influenced survival rates among Titanic passengers. The key insights derived were:

- **Gender**: The "women and children first" protocol [Birkenhead Drill](https://www.historic-uk.com/CultureUK/Women-Children-First/) significantly influenced survival rates, with females having a higher chance of survival despite being fewer in number. Males, while more numerous, experienced significantly higher mortality rates.
- **Class**: Socioeconomic status played a crucial role in survival outcomes. First-class passengers had the highest survival rates, reflecting their preferential access to lifeboats, while the majority of second- and third-class passengers faced devastating survival odds.
- **Age**: Younger children benefited from prioritization during evacuation, exhibiting the highest survival rates. Conversely, passengers aged 20-40 and the elderly experienced lower survival chances, influenced by physical challenges and situational disadvantages.
- **Family Size**: Passengers traveling alone or without children were the most vulnerable, particularly among elderly individuals. Those with one family member—such as a sibling or spouse—had improved survival rates, emphasizing the role of familial support during crises.
- **Fare and Socioeconomic Indicators**: Higher ticket fares correlated with greater survival likelihood, underscoring differences in access to lifeboats and resources based on economic status.
- **Embarkation**: While Southampton served as the primary point of embarkation, no significant relationship was found between embarkation location and survival outcomes.

## Logistic Regression

A logistic regression model was developed to predict survival outcomes based on passenger data. 

- **Accuracy**: The model achieves an accuracy of **81.46%**, indicating it can reliably predict survival for most passengers.
- **Precision and Recall**: Precision and recall scores demonstrate that the model performs well in identifying survivors (class 1) and non-survivors (class 0). 
  - Precision is **75%** for survivors and **86%** for non-survivors, with an average precision of **82%**.
  - Recall shows the model successfully identifies survivors **78%** of the time and achieves an overall recall of **81%**.
- **F1 Score**: The model’s F1 score of **82%** represents a balanced measure of precision and recall.

## Dataset

The dataset used in this analysis comes from the [Kaggle Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset). This data includes detailed records of Titanic passengers, originally compiled by multiple researchers, including the comprehensive work of Eaton & Haas in *Titanic: Triumph and Tragedy* (1994).

## Installation Instructions

The code in this Github Repo is done with Python 3.11 you may follow the following steps to run the analysis.

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