# Music Recommendation System

This project develops a **personalized music recommendation system** that combines clustering and classification techniques to improve how users discover songs on streaming platforms like Spotify.

## Project Overview

* **Exploratory Data Analysis (EDA):** Cleaned and explored over 100,000 tracks, focusing on key audio features (danceability, energy, tempo, valence, etc.).
* **Clustering:** Used **K-Means** to group songs into clusters with distinct characteristics (e.g., upbeat dance tracks, mellow acoustic songs). Evaluated optimal `k` with the Elbow Method and Silhouette Score.
* **Classification:** Trained a **K-Nearest Neighbors (KNN)** classifier to predict cluster labels for new songs, achieving **95.6% accuracy** with a strong Kappa score (0.93).
* **Recommendation Engine:** Recommended similar songs based on audio features, demonstrating the ability to generate relevant, diverse suggestions.

## Why this matters

Traditional music recommendation algorithms often rely only on user history, which can miss evolving tastes. By focusing on **audio features** and combining clustering with classification, this project shows how to provide both **accurate** and **diverse** recommendations.

## Skills Demonstrated

* **Data Cleaning & Preparation:** Handling duplicates, transforming variables, scaling features.
* **Exploratory Data Analysis:** Correlation analysis, outlier detection, distribution visualization.
* **Unsupervised Learning:** K-Means and DBSCAN clustering.
* **Supervised Learning:** KNN classification with hyperparameter tuning and cross-validation.
* **Evaluation:** Confusion matrices, accuracy, Kappa scores, sensitivity/specificity.
* **Recommendation Systems:** Building a feature-based recommendation engine.

## Tools & Technologies

* **R / RStudio**
* R packages: `caret`, `FNN`, `factoextra`, `dbscan`
* Dataset: [Spotify Tracks Dataset on Kaggle](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)

## Repository Contents

* **`Classification_final.Rmd`** – R Markdown notebook with full code (EDA, clustering, classification, recommendation system).
* **`Group136_Project_Report_V1.pdf`** – Final report with detailed methodology, results, and visuals.
* **`dataset.csv`** – Cleaned subset of Spotify dataset used for analysis.

## Key Results

* K-Means with **4 clusters** provided the best balance of compactness and separation.
* KNN classifier achieved **95.59% accuracy** in predicting song clusters.
* The system generated meaningful recommendations (e.g., classical music input → classical/acoustic recommendations).

## Lessons Learned

* The importance of feature engineering and scaling for high-dimensional datasets.
* Combining **unsupervised + supervised learning** can provide both interpretability and predictive power.
* Working with large datasets requires strategies to manage memory and computation limits.

## Credits

Project completed through the Data Mining and Statistical Learning class (ISYE 7406) at **Georgia Tech**, by my group and I:

* Diane Egret
* Arya Divakaran Kalappurayil
* Linggan Chen
