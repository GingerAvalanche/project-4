# Project-4

## Overview

Heart disease accounts for 1 in every 5 deaths in America every year. Being able to predict the onset of heart disease would be a great boon to the medical industry, allowing patients to avoid costly treatments by using relatively low-cost preventatives.

This project aims to use data concerning other, related health factors, along with a logistic regression learning model to determine the likelihood of the present of heart disease in a patient.

## ETL

The data, which has already been used for similar purposes before by other researchers, was already in mostly-appropriate format for analysis. However, there were a few problems that we had to overcome:

##### Significance of duplicates

There were duplicates in the heart disease data set, which we decided to remove after determining that these combinations of data should be so unique duplicates would be errors.

##### Presence of incorrect cholesterol values

There were many points of data where the cholesterol value - a value that should never be zero - was, in fact, zero. We determined that this was in error, but left that data in the set so that we could utilize its other properties.

##### Data format and visualization

The data was formatted well for machine learning. However, visualization was another matter, so we created a duplicate dataset with the legend values imported directly.

## The Cloud

This dataset was not extensive enough to require cloud computing. However, there were aspects of the project (such as regression model tuning) that made it advantageous to run it in the cloud, so we utilized AWS and Google Colab for those purposes.

## Heart Disease Importance

https://public.tableau.com/app/profile/alejandra.bridegroom/viz/HeartDiseaseProject_16987257944330/Story1?publish=yes

As mentioned, heart disease is responsible for almost 20% of all deaths in America.

(Say something here about specific visualizations, and their importance to local communities. Something about Tulare, Guam, Mississippi - and perhaps Michigan ;) - would work)

## Machine Learning

We used logistic regression for the model, due to the multiple non-continuous features in our data set.

As mentioned, there was erroneous cholesterol data. We had thought that including that data might decrease the accuracy of our models. However, this was emphatically not the case: of the top 10 feature sets for model accuracy, cholesterol was included in the top 8 sets. In addition, removing the cholesterol feature caused accuracy of those sets to drop by a flat 10% across the board. We believe that obtaining a larger data set with more accurate cholesterol levels would be incredibly advantageous to any future models.

## Conclusion

We were able to obtain 86% accuracy, precision, and recall ratings for our learning model. While very good, we do not believe that this is quite good enough for general use: in the public health arena, telling 14% of people that they were falsely identified (either positively or negatively) for heart disease is just too high a margin of error.

However, the insufficiencies in the data set do suggest that we are on the right track, and that the problem here is simply a matter of available data. Were more - and more complete - of the same amount of data to be made available, it is likely that we could achieve acceptable levels of accuracy.


### Sources
https://public.tableau.com/app/profile/alejandra.bridegroom/viz/HeartDiseaseProject_16987257944330/Story1?publish=yes

Rates and Trends in Coronary Heart Disease and Stroke Mortality Data Among US Adults (35+) by County – 1999-2018
https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Rates-and-Trends-in-Coronary-Heart-Disease-and-Str/9cr5-2tt7
