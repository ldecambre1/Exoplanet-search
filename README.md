# **Kepler Exoplanet Classification using Machine Learning and Neural Network Methods**

In this repository, we classify exoplanet candidates using data from NASA's Kepler Space Telescope, available [here](https://www.kaggle.com/datasets/nasa/kepler-exoplanet-search-results). This project demonstrates a full machine learning workflow, from data cleaning to model evaluation, using real astronomical observations.

We chose the Kepler dataset because it provides real-world astronomical measurements with noisy data, missing values, and class imbalance, making it an ideal case for comparing classical machine learning and neural network approaches.

## **Overview**

The aim of this project is to use classical **machine learning (ML)** and **neural network (NN)** approaches to classify Kepler Objects of Interest (KOIs) as **CONFIRMED**, **CANDIDATE**, or **FALSE POSITIVE**. By comparing traditional ML and NN approaches, we aim to explore the trade-offs between model interpretability, computational cost, and predictive accuracy when working with large, noisy datasets.

This project is split into three main sections:
* **Question 1**: Traditional ML classification using decision trees, evaluating performance and interpretability, and then improving model with ensemble methods (e.g, random forests).
* **Question 2**: NN classification using PyTorch, allowing comparison with ML results and exploring more complex patterns in the data.
* **Question 3**: Investigating how choices about data (e.g., amount of training data, class imbalance, feature selection) affect NN performance.

Each notebook (`question_1_notebook.ipynb`, `question_2_notebook.ipynb`, `question_3_notebook.ipynb`) is self-contained. Notebooks are structured as tutorials for beginners (Question 1, Question 2) or intermediate users (Question 3).

## **Goals**

* Compare ML and NN techniques for exoplanet classification.
* Understand how neural network design choices and dataset characteristics influence model performance.
* Identify which features are most informative for classification.
* Develop a reproducible machine learning workflow for analysing astrophysical datasets using Python.

## **Dataset**

The project uses the Kepler Space Telescope dataset, which contains ~10,000 KOIs with features describing both **stellar parameters** (e.g, effective temperature, radius, surface gravity) and **planetary candidate** parameters (e.g, orbital period, transit duration, transit depth, planetary radius). Key columns include:

| **Columns**        | **Descriptions**|
|----------------|-------------------------------------------------|
|kepoi_name      |Identifier for a Kepler Object of Interest (KOI).|
|kepler_name     |Assigned name for confirmed planets.|
|koi_disposition |Community's classification (CANDIDATE, FALSE POSITIVE, CONFIRMED).|
|koi_pdisposition|Kepler's internal pipeline classification using the same categories.|
|koi_score       |Confidence score (0-1) for classification with higher scores indicating higher confidence.|

This dataset is challenging due to noisy measurements, missing values, and overlapping class features, making it ideal for testing ML and NN approaches.

## **Dependencies**

* Python
* pandas
* numpy
* scikit-learn
* tensorflow
* matplotlib
* seaborn

## **Usage**

To clone this repository use: ```git clone https://github.com/ldecambre1/Exoplanet-search.git```

Make sure you ```pip install``` all the dependencies listed in ```dependencies.txt```, using ```pip install -r dependencies.txt```.

Follow the notebooks in order:
* `question_1_notebook.ipynb`: Train and evaluate decision tree and ensemble ML models.
* `question_2_notebook.ipynb`: Train and evaluate neural network models using PyTorch.
* `question_3_notebook.ipynb`: Investigate effects of dataset choices on NN performance.

## **License**

This project is listed under the MIT license, see ```LICENSE``` for more information.

## **Acknowledgements**

I would like to take a moment and thank the following for their assistance throughout the project:

* **[NASA Kepler Space Telescope](https://exoplanetarchive.ipac.caltech.edu/docs/KeplerMission.html)** for providing the dataset that made this project possible.
* **Coleman Krawczyk** for guidance on coursework structure and software engineer best practices.
* **Lysette Stubbs** for proofreading, support, and filling in gaps in my understanding.
* **[ChatGPT (OpenAI)](https://openai.com/index/chatgpt/)** for helping debug code and clarifying any tricky concepts.

## **Contact**
Lewis Decambre  
lhrdecambre@gmail.com  
MPhys Physics, Astrophysics and Cosmology  
University of Portsmouth  
