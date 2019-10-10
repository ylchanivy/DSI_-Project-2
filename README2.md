# Problem Statement:
To create a Linear Regression Model based on the Ames Housing Dataset to predict the price of a house.<br>
To Identify what are the features that will influence price of a house in Ames.

# Dataset:

Data set contains information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010.

All 7 csv data sets were saved in the repository 'datasets' folder. 


|File Name |Description |Number of Rows|Number of Columns|
|------|------|------|------|
|train.csv|original dataset were downloaded from Kaggle|2051|81|
|test.csv|original dataset were downloaded from Kaggle|879|80|
|train_clean.csv|train dataset that has all null value updated and additional 'train' column added|2050|82|
|test_clean.csv|test dataset that has all null value updated and additional 'train' column added|879|81|
|train_final.csv|train dataset that has dummy variable created and ready to be used for model training|2048|233|
|test_final.csv|test dataset that has dummy variable created and ready to be used for final model test|879|233|
|submission.csv|predicted test result that was submitted to Kaggle|879|2|


# Data Dictionary:

Refer to this link for full Data Dictinary:
http://jse.amstat.org/v19n3/decock/DataDocumentation.txt

Below is data dictionary for features was created

|Feature |Type |Description |
|------|------|------|
|Property Age|int|Current Year minus Year Built|
|Remodel Age|int|Current Year minus Year Remod/add|
|Remod/Add|int|Remod/Add: 1, No Remod/Add:0|
|Overall Qual*Exter Qual|int|Interaction Term between Overall Qual & Exter Qual|
|Lot Area*Remodel Age|int|Interaction Term between Lot Area & Remodel Age|
|Property Age*Lot Area|int|Interaction Term between Property Age & Lot Area|
|Gr Liv Area*TotRms AbvGrd|int|Interaction Term between Gr Liv Area & TotRms AbvGrd|



# Conclusion and Recommendations
Based on the score above, the top features 9.that influences House sale Price are: External Quality, Overall Quality,Interaction of External Quality & Overall Quality, Kitchen Quality,Garage Call, Basment Quality,Property Age, Year remodel/Add, Full Bath, found_pCon, Total Room Above Ground and FirePlace Quality.<br>
Removing features that shows '0'magnitude in lasso regression chart does not imporved the model score.
