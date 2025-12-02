# Kepler Exoplanet Search Results

This repository explores exoplanet data from NASA's Kepler Space Telescope with the goal of identifying, classifying and analysing potential exoplanets. This project builds a reproducible machine learning pipeline covering data preprocessing, feature engineering, model training and performance evalution.

# Project Overview

The purpose of this project is to demonstrate a complete, end-to-end data science workflow using real astronomical data. I have chosen exoplanet detection as it is a good example for this type of study as it combines noisy observational measurements with astrophysical context, creating a real scientific classification problem. In this project, the Kepler dataset is explored, cleaned and prepared for analysis, and then both classical machine learning (ML) and neural network (NN) methods are applied to classify planetary candidates.

Comparing these approaches is important because both have their distinct strengths. Traditional ML techniques, such as decision trees, are generally easier to interpret and faster to train, making it clear which features influence predictions. While neural networks, on the other hand, can capture more complex relationships in the data, but at the cost of being less transparent and requiring more computational resources. By applying both methods to the same dataset, this project highlights how different modelling approaches handle a real scientific problem and what trade-offs exists between interpretability and predictive power.

This project is developed under version control to follow good scientific computing practices and to ensure reproducibility. Overall, the goal is to show data sciences techniques can be applied to real astronomical datasets while providing insight into when and why different modelling approaches are useful.

# Objectives

The main objectives for this project are to explore the application of different machine learning techniques to a real astronomical dataset and to evalulate their effectiveness.

The project is divided into three main components, answering three questions:

**Q1:** Traditional ML techniques
In this section, we focus on classical machine learning methods. We explore how well a traditional approach performs in classifying exoplanets and consider ways to improve its accuracy. For this, decision trees are used to classify candidates as confirmed planets, candidates or false positives. This component highlights this interpretability and efficiency of traditional ML methods.

# Dataset

This project uses data from NASA's Kepler Space Telescope, which monitored over 150,000 stars in search of exoplanets using the transit method. The dataset, sourced from Kaggle is a catalogue of all observed Kepler "objects of interest", roughly 10,000 targets that showed transit-like signals worth investigating further. Each row corresponds to a planet candidate and includes its current classification along with a wide range of stellar and planetary parameters. 

This dataset includes several useful features describing stellar parameters such as effective temperature, surface gravity, and radius, and planetary candidate parameters including orbital period, transit duration, transit depth and planetary radius.

From a practical perspective, this datset is challenging as it contains noisy measurements, missing values and overlapping characteristics between classes, all issues that astronomers regularly deal with. By preparing and analysing this data, this project provides an opportunity to explore how different machine learning approaches handle these challenges and which features are most informative for classifying planetary candidates.

This dataset can be found at: https://www.kaggle.com/datasets/nasa/kepler-exoplanet-search-results

A few notable columns include:

* kepoi_name: The identifier for a Kepler Object of Interest (KOI). A KOI shows at least one transit-like signal that appears astrophysical and could plausibly be a planet.
* kepler_name: The assigned name for candidates that have been promoted to confirmed planets.
* koi_disposition: The community’s current classification of the candidate (CANDIDATE, FALSE POSITIVE, or CONFIRMED).
* koi_pdisposition: Kepler’s internal pipeline classification using the same categories.
* koi_score: A value between 0 and 1 indicating confidence in the classification. For CANDIDATES, a higher score means higher confidence; for FALSE POSITIVES, a higher score means lower confidence.







