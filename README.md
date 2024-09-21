# NBA Career Retention Prediction

This project creates a machine learning model that predicts NBA career retention based on a player’s rookie year performance. The model is designed to help recruiters and team managers make informed decisions about player investments, as well as assist audiences in predicting player performance for betting purposes.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Description](#data-description)
3. [Model](#model)
4. [Results](#results)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Future Work](#future-work)
8. [Technologies Used](#technologies-used)
9. [Disclaimer](#disclaimer)
10. [Contact](#contact)

## Introduction

NBA recruiters, team managers, and even fans invest heavily in predicting a player's career potential. This project aims to streamline that process by developing a predictive machine learning model based on rookie-year statistics to determine whether a player will remain active in the league. With the average NBA player's salary at $10.8 million, identifying future star players can help teams make more strategic investments (Fisher, 2023). For fans and bettors, this model provides insights for better decision-making when predicting outcomes in NBA games.

## Data Description

We used two datasets scraped from [Sports Reference](https://www.sports-reference.com/) that contain NBA player statistics for a given basketball season. We focused on the following seven metrics:
- Age
- Years played
- Games played
- Total minutes played
- Minutes played per game
- Total points
- Points per game

Due to licensing restrictions, we cannot publicly share the data. However, links to the original data sources are provided. Data cleaning and processing were performed to label players as either "active" or "inactive" based on career status.

## Model

We implemented a **supervised logistic regression model** for predicting player retention. Logistic regression was chosen as it is a binary classifier, making it ideal for our data, which categorizes players as "active" or "inactive."

### Model Workflow:
1. Web scraping of NBA player data.
2. Data cleaning and preparation.
3. Training the logistic regression model.
4. Evaluation using classification reports and **K-fold cross-validation**.
5. Testing with five distinct test cases.

## Results

- **Accuracy**: The model provided a general classification accuracy score and was further validated using K-fold cross-validation for deeper insights.
- **Error testing**: We performed tests on the model’s performance to identify any potential errors and directions for future improvements.

## Installation

To run this project locally:

```bash
# Clone the repository
git clone https://github.com/your_username/nba-career-prediction.git

# Navigate to the project directory
cd nba-career-prediction

# Install dependencies
pip install -r requirements.txt
