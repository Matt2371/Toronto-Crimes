# Toronto-Crimes
Analysis of major crimes in Toronto using data from the Toronto Police Service, which includes 323,296 crimes between 2014 and 2022 and various variables about the time and location of the reported crime. Initially, we explored temporal and geospatial crime patterns using exploratory data analysis, interactive maps, and unsupervised association rule mining. Notably, we found a high frequency of auto thefts in West-Humber Clairville and a high frequency of assaults in Moss Park. Next, we employed association rule mining to uncover key associations between the different variable conditions and crime type that appear frequently in the data. By doing so, we found a strong association between apartment locations on the weekend and assault crimes.<br/>

In the next section, we explored predictive analytics, that is, predicting crimes based on the various time and location features. First, we modeled the multiclass prediction problem of classifying crime type (assault, auto theft, break and enter, etc...). Using multiclass logistic regression as a baseline (which assumes linearity), we compared the performance of random forest and gradient boosted trees (xgboost) using the f1 score, accuracy score, precision, and recall. All the models suffered when predicting minority crime types, even after measures were taken to account for the class imbalance such as class weighting, bootstrap clas weighting, and minority class oversampling. Thus, we concluded that the data does not discriminate between the different crime types well (except for assault). With this in mind, we focused on the binary classification problem of predicting assaults using decision trees, with the choice of decision trees stemming from its high interpretability and nonlinear capacity. Such decision trees performed reasonably well on all metrics.<br/>

<br/>

# Notebooks
1. EDA.ipynb: Exploratory data analysis and interactive maps in Folium. 
2. data_processing.ipynb: Data cleaning and feature engineering
3. predictive_modeling.ipynb: Multiclass and binary crime classification
4. association_rule_mining.ipynb: Assocition rule mining.

# Other files and folders
data/ : stores raw data obtained from https://data.torontopolice.on.ca/datasets/TorontoPS::major-crime-indicators-open-data/explore. Not included in repository. <br/>
html/ : stores html interactive heatmaps of crime density by type <br/>
figures/ : static visualizations from EDA <br/>
Final_report.pdf : final report detailing methods and results
PSDP_Open_Data_Documentation.pdf : official data source documentation
