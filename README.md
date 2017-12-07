# 50-Bootstrap-Cross-Validation-for-Predicting-Mental-Health-Emergency-Department-Presenation-Rates
Some code for our our linear-mixed-model predictions using LMM's

During my last semester I worked with the Collaborative for Health Analysis and Statistical Modelling. I aided them in creating a cross-validation algorithm to find the optimal linear mixed effects model for predicting mental health emergency department rates for young adults in West Australian suburbs. We created a list of all possible variables, and from that a list of all possible models. We then trained the models on 10 years of past data and tested the model predictions on test data 3-5 years in the future using 5-fold cross validation with 50 bootstraps.

This kind of algorithm could be used on any large enough data set to predict binary outcomes based on any number of features or variables. If you look deep into the code you can see we compare 527 possible models for prediction, obtain PPV's and Sensitivities for our test sets (which allow us to estimate each models performance) and then are able to select an optimal model.

The optimal model in this case had an 80% PPV at a 40% Sensitivity threshold meaning that 80% of the positive predictions for high rates of mental health emergency presentation rates were correctly predicted.

As this analysis was quite in depth and technical, please contact me via e-mail if you are interested in the full 20-page report. The data used in this analysis is only accessible at a specific location. Therefore this code is here to display the general framework to create a predictive model using longitudinal data points.
