# Breaking the Glass Ceiling: Looking at Glass Type Classification
## Final Project, Launchcode Women+ Fall 2021 Cohort

### Collaborators:

Nasiba Adilova, Heather Leighton-Dick, Madison Massie


## Overview
Glass is a fascinating substance: a solid material with the molecular structure of a liquid. Glass occurs naturally in the world, usually as the byproduct of a natural phenomenon like molten lava or a lightning or meteor strike. Humans have been making glass since about 3600 BC, and initially used it for decoration and food storage/serving. Today, glass is used around the world in many different chemical variations and in many different industries (medicine, technology, building construction, and construction, to name a few). The word "glass" usually refers to materials that are at least 70% silicate, but the presence or absence of other materials such as barium, iron, calcium, and sodium create different types, or classes, of glass which share physical properties. Classifying glass means being able to predict its physical qualities from its chemical makeup, as well as being able to figure out its source from its physical qualities.

## Project Description
  Our objective was to create and compare models that could be used to predict a glass's type, and to discover which model is most accurate. The dataset came from the University of California Institute of Machine Learning via Kaggle (https://www.kaggle.com/uciml/glass), and is comprised of 10 columns:
  
  1 - Refractive Index, which is the 
  
  2–9 Formers, Fluxers, Stabilizers: substances that make up the composition of the glass sample
  
  10 - Type of Glass (Type 1–7) [the prediction target]
  
Since types 1 and 2 represent a majority of the observations in the dataset, we chose to test multi-classification models which would perform decently with imbalanced data, and resampled the data to help represent the minority classes.

## Key Techniques

 Pandas: downloading the dataset and importing into a dataframe,
          cleaning and renaming columns
          
 Standar Scaler: make sure all the columns are standardized

 SMOTE resampling: adding similar minority datapoints to help represent minority glass types 

 Sklearn: 
 
 -- Train-test-split, using the same random state (42) and test size (20%) for every model
 
 -- Accuracy and ROC scores
 
 -- ROC AUC curves
 
 -- Confusion matrices

 ## SQL: ETL: Create A Database

<img width="512" alt="data ER model" src="https://user-images.githubusercontent.com/91164907/157516358-5c51d93d-ff12-4416-8c6d-d784e441d10b.png">


## SQL Queries

What is the most common chemical element in glass?

Which element is the least common?

Is there an element present that doesn’t change a glass sample’s type?

Which model performed best when comparing observed type to predicted type?


## Trying Different Models

Madison – ANN, KNN

Heather – SVM (Linear, RBF, Polynomial)

Nasiba – RandomForest

## Lessons Learned 

The dataset doesn’t have any examples of Type 4, so we had to decide how to handle that class, whether to include it. 
Research showed that Type 4 is typically made through a non-float process which is less common now and largely absent from commercial
production, so we decided to ignore the class and focus our predictions on the other types of glass.


## Conclusions
![bargraphaccuracy](https://user-images.githubusercontent.com/91164907/157535812-fc9b3810-4cc9-4e93-96da-1b1ac45e062c.jpg)

The RandomForest multi-classification model performed the best overall,

Why might that be? ???


What was your motivation?
Why did you build this project?
What problem does it solve?
What did you learn?
What makes your project stand out?


Why is glass important to study?  Medical applications, information technology, crime scene forensics, architecture 


what would you add/change/enhance in the future? 


## License

This project is licensed under the terms of the MIT license.

## Helpful Links

Corning Museum of Glass: 
https://www.cmog.org/article/chemistry-glass

ScienceDirect:
https://www.sciencedirect.com/topics/materials-science/glass-composition

Encyclopedia Britannica:
https://www.britannica.com/technology/glass

Wikipedia:
https://en.wikipedia.org/wiki/Glass

Nature: Scientific Reports: article on glass scaffolding for bone regeneration
https://www.nature.com/articles/srep19361

How to Write a Good Readme: 
https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/

