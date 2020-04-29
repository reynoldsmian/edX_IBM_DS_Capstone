# edX_IBM_DS_Capstone

This is the original run through for edx Data Science and Machine Learning Capstone Project. 

## Problem Statement

The people of New Yorker use the 311 system to report complaints about the non-emergency problems to local authorities. Various agencies in New York are assigned these problems. The Department of Housing Preservation and Development of New York City is the agency that processes 311 complaints that are related to housing and buildings.

In the last few years, the number of 311 complaints coming to the Department of Housing Preservation and Development has increased significantly. Although these complaints are not necessarily urgent, the large volume of complaints and the sudden increase is impacting the overall efficiency of operations of the agency.

Therefore, the Department of Housing Preservation and Development has approached your organization to help them manage the large volume of 311 complaints they are receiving every year.

The agency needs answers to several questions. The answers to those questions must be supported by data and analytics. These are their  questions:

Which type of complaint should the Department of Housing Preservation and Development of New York City focus on first?
Should the Department of Housing Preservation and Development of New York City focus on any particular set of boroughs, ZIP codes, or street (where the complaints are severe) for the specific type of complaints you identified in response to Question 1?
Does the Complaint Type that you identified in response to question 1 have an obvious relationship with any particular characteristic or characteristics of the houses or buildings?
Can a predictive model be built for a future prediction of the possibility of complaints of the type that you have identified in response to question 1?
Your organization has assigned you as the lead data scientist to provide the answers to these questions. You need to work on getting answers to them in this Capstone Project by following the standard approach of data science and machine learning.

The notebooks were split up into the four questions of the project: 
* Q1 - Identify the top complaint type
* Q2 - Identify areas most affected by the top complaint type
* Q3 - Identify relationships between building characteristics and the top complaint
* Q4 - Create a model to predict the top complaint type

## Datasets 

**311 complaint dataset**
* This dataset is available at https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9. You can download part of this data by using SODA API.
* Only the data that is related to the Department of Housing Preservation and Development was analyzed

**PLUTO dataset for housing**
* This dataset for housing can be accessed from https://data.cityofnewyork.us/City-Government/Primary-Land-Use-Tax-Lot-Output-PLUTO-/xuk2-nczf. 
* Only the data for the borough of interest was imported 

**Borough boundaries geojson**
* Available from https://data.cityofnewyork.us/City-Government/Borough-Boundaries/tqmj-j8zm

## Packages
* Pandas
* Numpy
* matplotlib
* seaborn
* sklearn
* tensorflow

# Project Notes:

Original csv is too large to upload on Github so first notebook cannot be run from scratch. Pkl files for Q2, Q3, and Q4 are included. 

Future work:
- The unbalanced nature of the data lead to over predicting of negative results. The weighted F1 score of 0.83 is not terrible, but further feature engineering and tweaking to the model must be done in order to increase recall on the positive results. 
