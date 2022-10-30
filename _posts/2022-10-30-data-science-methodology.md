---
title: Data Science Methodology.
date: 2022-10-30 12:00:00 +300
categories: [IT]
tags: [data science]
---
# Data Science Methodology

Nowadays, we are observing how data became one of the important assets to a company. This is an issue that follows the advances of both hardware and software technologies and the growing online presence of the people and the markets of the past years, which enables data collection as we never saw before. The importance of the data lies in the patterns that can be traced back to a company's status and behaviors. Many problems can be solved by exploring these patterns but only if we have a good methodology.

Concerning the efficiency of many decisions to turn the data into insights for the stakeholders, an organized approach must be set, with clear descriptions of each step and task involved. This discussion is inspired by Coursera's Data Science Methodology from IBM, which is one of those recommended to newcomers in the Data Science field. Among the methodologies, the course focus on John Rolling's approach, who is one of the leading Data Scientists at IBM, and the steps are shown in the figure below.

<p align="auto">
<img width="80%" height="auto" src="/assets/lib/images/methodology.jpg"/>
</p>

The methodology has three main tasks: first is the problem approach, where an initial investigation is done, second is the collection and process of the data and third, deriving answers through models and evaluating them. This text deals with these matters in a generalized way, not picking a specific model.

## 1. From Problem To Approach.

The importance of the first approach is to understand the problem clearly and to summarize the key points in questions to be answered like:

What is the problem you are trying to solve and how can you use data to answer it?

Depending on the problem, other stakeholders have to be addressed to clarify the questions. It's crucial to gain domain understanding with a review of the recent literature about the problem. It helps to identify what information we need, the source of the data and which patterns can we get from the data to address the questions most effectively.

Moreover, the importance to be careful with the first step is that any bad decision here can be time-consuming because all the subsequent work will depend on this information.

## 2. Working with data

Once the data scientists know what's the problem, the team handles the possible sources of information, formats, and storage.  The key question is: Are the sources available or do we have to arrange a data collection? Afterward, the material normally is not in shape for use and needs transformation. The phase of preparation to posterior use includes:

1. Formatting;

2. Identifying missing or invalid values;

3. Removing duplicates.

Decisions on what to do with the missing or invalid information have to be taken and how it affects the dataset is considered.

The prepared material now can be studied through methods like descriptive statistics to understand if its representative of the problem to be solved. Univariate statistics can be run through each variable to get, for example, the mean, median, standard deviation, maximum and minimum values. Second, a pairwise correlation can be done to see if the variables are correlated and which ones are too correlated, expressing redundancy.

A step further is feature engineering, which is to apply the domain knowledge to create features, or characteristics, that helps to solve the problem. It's critical when machine learning tools are been used.

## 3. Modeling and Evaluation

Modeling focus on developing descriptive or predictive models. The descriptive models examine the preference of behavior and probabilities of actions, whereas the predictive ones, what happens in the future based on patterns and can be done through statistics or machine learning.

To prove the model, the dataset is divided into training and test sets. The training set calibrates our model to be effective on the test set. Typically, several models are tested using the default parameters and then fine-tuned or revert to the data preparation phase for manipulations required by their model of choice.

After completing the models correctly, the results are evaluated with the selected criteria. The best models are selected and their findings are documented.

## 4. Deployment

The methodology is an iterative process and all the previous work affects the results of the test set. Hence, many modifications of the feature engineering may be done until achieving the required performance. If the results meet the criteria, the model is deployed.

Deployment means using the insights of the model with new real-life data for the stakeholders. The results are continuously monitored formal tasks such as final reports and project overviews can be necessary. 