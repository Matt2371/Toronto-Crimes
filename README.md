# Toronto-Crimes
Analysis and modeling of major crime in Toronto using data from the Toronto Police Service, which includes 323,296 crimes between 2014 and 2022 and various variables about the time and location of the reported crime. We present the following key analysis: <br/>

1. Interactive maps and figures to learn geographic and temporal crime patterns.
2. Multiclass crime prediction: prediction of crime type given time and location variables. Compared performance between Multiclass Logistic Regression, Random Forest, and Gradient Boosted Trees. Conducted sample weighting and oversampling to deal with class imbalances.
3. Binary crime classification: interpretable prediction of assault crimes using a high performance Decision Tree
4. Association Rule Learning to uncover key associations between the different variable conditions and crime type that appear frequently in the data

<br/>

# Folders
data/ : stores raw data obtained from https://data.torontopolice.on.ca/datasets/TorontoPS::major-crime-indicators-open-data/explore. Not included in repository.

# Notebooks
1. EDA.ipynb: Exploratory data analysis. 
2. data_processing.ipynb: Data cleaning and feature engineering
3. predictive_modeling.ipynb: Multiclass and binary crime classification
4. association_rule_mining.ipynb: Assocition rule mining.

