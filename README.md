# Breaking the Glass Ceiling: Looking at Glass Type Classification
## Final Project, Launchcode Women+ Fall 2021 Cohort

### Collaborators:

Nasiba Adilova, Heather Leighton-Dick, Madison Massie


## Overview
Glass is a fascinating substance: a solid material with the molecular structure of a liquid. Glass occurs naturally in the world, usually as the byproduct of a natural phenomenon like molten lava or a lightning or meteor strike. Humans have been making glass since about 3600 BC, and initially used it for decoration and food storage/serving. Today, glass is used around the world in many different chemical variations and in many different industries (medicine, technology, building construction, and construction, to name a few). The word "glass" usually refers to materials that are at least 70% silicate, but the presence or absence of other materials such as barium, iron, calcium, and sodium create different types, or classes, of glass which share physical properties. Classifying glass means being able to predict its physical qualities from its chemical makeup, as well as being able to figure out its source from its physical qualities.

## Project Description
  Our objective was to create and compare models that could be used to predict a glass's type, and to discover which model is most accurate. The dataset came from the University of California Institute of Machine Learning via Kaggle (https://www.kaggle.com/uciml/glass), and is comprised of 10 columns:
  
  1-Refractive Index
  
  2-9 Substances
  
  10-Class (Type 1–7)
  
Since types 1 and 2 represent a majority of the observations in the dataset, we chose to test multi-classification models which would perform decently with imbalanced data, and resampled the data to help represent the minority classes.
  
  
  
## Key Topics/Table of Contents

Key Techniques

 Pandas: downloading the dataset and importing into a dataframe,
          cleaning and renaming columns
          
 Standar Scaler: make sure all the columns are standardized

 SMOTE resampling: adding similar minority datapoints to help represent minority glass types 

 Sklearn: Train-test-split, using same random state (42) and test size (20%)
          accuracy and ROC scores, ROC AUC curves, confusion matrices

 SQL: ETL, create a database
![data%20ER%20model.png]

### trying different models


Madison – ANN, KNN

Heather – SVM (Linear, RBF, Polynomial)

Nasiba – RandomForest


## Conclusions

  some of the challenges you faced
  
  what would you add/change/enhance in the future?
  
Which model performed the best overall? Based on accuracy score

Why might that be? ???

Why is glass important to study?  Medical applications, technology, crime scene forensics, architecture 


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



What was your motivation?
Why did you build this project?
What problem does it solve?
What did you learn?
What makes your project stand out?
If your project has a lot of features, consider adding a "Features" section and listing them here.




SQL Queries:
What is the most common chemical element in glass?
Which element is the least common?
Is there an element present that doesn’t change a glass sample’s type?
Which model performed best when comparing observed type to predicted type?

Lessons Learned: --data doesn’t have any examples of Type 4 (found out half-way through)


