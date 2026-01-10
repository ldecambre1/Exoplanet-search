# **Kepler Exoplanet Classification**
---

In this repository, we classify exoplanet candidates using data from NASA's Kepler Space Telescope, available here

# **Overview**
---

The aim of this project is to use classical machine learning (ML) and neural network (NN) approaches to classify Kepler Objects of Interest (KOIs) as **CONFIRMED**, **CANDIDATE**, or **FALSE POSITIVE**. By comparing traditional ML and NN approaches, we aim to find the the best solutions for handling large, noisy astronomical datasets.

The project is split into three main sections:
* **Question 1**: Traditional ML classification using decision trees, evaluating performance and interpretability, and then improving model with ensemble method.
* **Question 2**: NN classification, using PyTorch, allowing comparsion with ML results.
* **Question 3**: Investigating how choices about data (e.g., amount of traing data, class imbalance) affect NN performance.

# **Goals**
---

* Compare ML and NN techniques in exoplanet classification.
* Understand how neural network parameters and dataset characteristics influence performance.
* Develop a reproducible machine learning workflow for astrophysical datasets.

# **Dataset**
---
The project uses the Kepler Space Telescope dataset, which contains ~10,000 KOIs with features describing both stellar parameters (e.g, effective temperature, radius, surface gravity) and planetary candidate paramters (e.g, orbital period, transit duration, transit depth, planetary radius). Key columns include:

| Columns | Descriptions |
|---------|--------------|
|kepoi_name|Identifier for a Kepler Object of Interest|
|kepler_name|Assigned name for confirmed planets|
|koi_disposition|Community's classification (CANDIDATE, FALSE POSITIVE, CONFIRMED)|
|koi_pdisposition|Kepler's internal pipeline classification|
|koi_score|Confidence score (0-1) for classification|

This dataset is challenging due to noisy measurements, missing values, and overlapping class features, making it ideal for testing ML and NN approaches.

# **Dependencies**
---
* Python
* pandas
* numpy
* scikit-learn
* tensorflow
* matplotlib
* seaborn

# **Usage**
---

To clone this repository use: git clone https:github.com/ldecambre1/Exoplanet-search.git

Make sure you pip install all the dependencies listed in dependencies.txt, using !pip install (library)

# **License**:
---
This project is listed under the MIT license, see LICENSE for more information.

# **Acknowledgements**




