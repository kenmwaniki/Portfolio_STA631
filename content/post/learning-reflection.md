---
date: "2025-04-15T13:09:13-06:00"
title: Reflection on Learning and Participation
---

Reflection on Learning and Participation

## Course Learning Objective 1:  Describe probability as a foundation of statistical modeling, including inference and maximum likelihood estimation

For several of the assignments — specifically HomeWork 1 (HomeWork1SLR),  MLR  (Home Work 2),  Homework 4 (multinomial)and the GLM Cross-Validation Project  — I demonstrated how these basic concepts of probability are used to construct, test, and explain statistical models. This clearly demonstrated my understanding of confidence intervals, p-values, and maximum likelihood estimation (MLE), which I also expand on in my first reflection.

As I mentioned in Homework 1, one of my learning outcomes upon modeling the relationship between horsepower and mpg was interpreting p-values and confidence intervals. The p-value for horsepower was statistically significant (p < 0.0001), describing a negative relationship. Read about the importance of the assumption of normality of residuals, upon which the trustworthiness of inferential statistics builds.

In Homework 2, I built on this work to accommodate multiple predictors and to use MLR—reinforcing my foundation in inference. I interpreted significance for multivariable, and learned about collinearity and its affect on confidence of estimates.

Homework 4 presented multinomial logistic regression (Section 2), estimated using MLE. Using variables including age, education and income, I modeled the probability of each of the different categories of voter behavior, treating “rarely/never” as the baseline. I analyzed log-odds and then transformed them back into odds ratios, showing how I leverage probabilistic reasoning to make sense of category likelihoods.

Lastly, in the GLM Project and HW 5 (Cross Validation) I used cross validation to generalize model performance on an unseen data set using fold-wise sampling to calculate RMSE and residual variance. It is a sign of my increasing fluency in expressing uncertainty and variability probabilistically.

## Course Learning Objective 2: Determine the suitable generalized linear model (GLM) for a data context

This was shown in Homework 3 , Homework 4 (multinomial), and the GLM Project . For each, I analyzed the structure of the data, chose the appropriate GLM, and implemented appropriate preprocessing and modeling workflows in R.

I used logistic regression to model binary outcomes with categorical predictors in Homework 3. I did dummy encoding, carefully chose reference levels, and interpreted coefficients in terms of odds ratios.

In homework 4, I switched to a multinomial logistic regression with a three-category outcome variable (voter behavior). I went with the multinom_reg() function from tidymodels, specified the right category to be the baseline, and interpreted the output with odds ratios — demonstrating solid knowledge of the appropriate GLM for unordered categorical outcomes.

I reported my logistic regression analysis of SEGRADES, a binary academic performance outcome, in the GLM Project (Sections 1–3). I did some data cleaning and encoding, used vfold_cv for resampling. By using accuracy metrics, I validated model performance, stressing the consistency of model type with data type.

## Course Learning Objective 3: Given a set of candidate models, demonstrate model selection

This was a major focus in Homework 5 (Cross Validation), Homework 6, and the GLM Project 

In Homework 5, I first built models having single predictors such as horsepower, followed by building multivariable regression models. I performed forward and backward stepwise selection and assessed models based on adjusted R², RMSE, and residual analysis. This rule helped me optimise the complexity of models we train with performance.

I used polynomial regression for Homework 6 and step_poly() to tune variable degrees. I tested many combinations in parallel to do so efficiently. I selected final models by RMSE, explored the marginal impact of polynomial terms, and realized the price of multicolinearity.

In the GLM Project : I used v-folds cross validation to compare multiple predictor sets. I added theoretically important variables (such as behavioural indicators) and ultimately selected a final model based on performance and interpretability. This project established model selection as statistical both in principle and in application.

## Course Learning Objective 4: Convey the outcomes of statistical models to a lay audience

I did this in HomeWork 3 & Project 1 . Both called for explaining categorical and logistic models to those lacking technical knowledge.

Homework 3 includes a plain English explanation of coefficients for factor variables. Instead of simply reporting statistical values, I transformed the numbers into meaningful information in the real-world craft of odds ratios — something like “Group A is more likely than the reference group to experience the outcome.”

For Project 1, I created logistic models and visualized them using ggplot2 Using broom output, I summarized model accuracy, confusion matrices, and significant predictors. My writing had graphics and language for non-statisticians, including school officials and policymakers. This underscored that delivering meaningful insight is as important as accuracy in statistics.

## Learning Objective 5: Identify and use programming software for fitting and evaluating statistical models

In this course, I used R and tidymodels extensively to develop, tune, and evaluate models. I showed this in Homework 2 , Homework 6 , and the GLM Project.

In Homework 2, I created a full modeling pipeline using workflow() and recipe(), and then split the Auto dataset into train/test... Have found parsers for normalization of predictors, used MLR to fit models, metrics() and collect_predictions() for performance.

For Homework 6, I used step_poly() to tune polynomial degrees and used cross-validation to assess and select the best configuration.

In the GLM Project, I created a logistic model, used vfold_cv for resampling, used proper factor releveling, and assessed performance via AUC and accuracy. I constructed a single pipeline for data wrangling, model fitting and validation. This confirmed for me that I was ready to build full modeling workflows in R.