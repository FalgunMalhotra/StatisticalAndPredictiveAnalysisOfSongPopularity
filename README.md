# Statistical And Predictive Analysis Of Song Popularity

- [Statistical And Predictive Analysis Of Song Popularity](#statistical-and-predictive-analysis-of-song-popularity)
  - [Team](#team)
  - [Problem Statement](#problem-statement)
  - [Implementation](#implementation)
  - [Dataset](#dataset)
  - [Steps to Run](#steps-to-run)
    - [1. Clone the repository](#1-clone-the-repository)
    - [2. Install the necessary packages](#2-install-the-necessary-packages)
    - [3. Run jupyter notebook](#3-run-jupyter-notebook)
  - [References](#references)


## Team
 
 - Advaith Rao
 - Ayush Oturkar
 - Falgun Malhotra
 - Hsiao-Chun Hung
 - Vanshita Gupta

## Problem Statement

The objective of conducting this analysis was to build a robust model to predict the popularity of a song based on several attributes like energy, acoustics, tempo, liveness, danceability, as well as to understand how these features impact it.

To achieve this goal, we worked on the following tasks (but not restricted to):

- Exploratory Data Analysis
    - Check feature importance
    - Correlation matrix
    - Detect Anomalies (If any)
- Data Cleaning and Feature Engineering
    - Check for Multicollinearity (If any)
    - Perform test for outlier removal (If any)
    - Find and Impute missing values (If any)
    - Check for influential and leverage points
    - Add new features(If any)
- Model Development and Fine-tuning 
    - Feature Selection using forward or backward elimination (If required)
    - Q-Q plot to check for residual normality
    - Perform Residual Analysis
    - Variable Transformation (If any)
- Hypothesis Testing
    - Understand feature significance and its impact on song popularity
    - Comparison with other complex models

## Implementation

Kindly find our implementation in this IPython notebook [here](https://github.com/FalgunMalhotra/StatisticalAndPredictiveAnalysisOfSongPopularity/blob/main/Notebook/main.ipynb).

## Dataset
 
We use the Spotify Audio Features dataset, which uses the open-source native Spotify API to collect certain audio features for song popularity analysis. The dataset could be found [here](https://www.kaggle.com/datasets/tomigelo/spotify-audio-features).

The description for the different variables used in our dataset can be found on the [Spotify developer API page](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features)

## Steps to Run

### 1. Clone the repository

```git clone https://github.com/FalgunMalhotra/StatisticalAndPredictiveAnalysisOfSongPopularity.git```

### 2. Install the necessary packages

**2.a. Create a virtual environment**

```python3 -m venv <env_name>```

**2.b. Source onto that environment**

```source <env_name>/bin/activate```

**2.c. Pip install the necessary packages**

```pip3 install --upgrade pip | pip3 install -r requirements.txt```

### 3. Run jupyter notebook

Start a jupyter notebook session and run the desired experiment.

```jupyter notebook```
 
## References

[1] https://github.com/tgel0/spotify-data - Github repository containing track information data fetch from Spotify using Spotify API

[2] https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features - Description of the different variables we use in our dataset.

[3] https://www.frontiersin.org/articles/10.3389/fpsyg.2018.02118/full - Effects of tempo as an emotional feature on music listeners. We used this as a reference to binning tempo into categorical variables of slowtempo(-1), mediumtempo(0) and uptempo(1)

[4] https://github.com/scikit-learn/scikit-learn - Scikit-Learn package for data cleaning and modeling in python.

[5] https://github.com/statsmodels/statsmodels - Statsmodels package for Regression.

[6] https://github.com/catboost/catboost - Catboost package for fast, scalable Boosting-based
Regression in Python.

[7] https://desktop.arcgis.com/en/arcmap/latest/extensions/geostatistical-analyst/normal-qq-plot-and-general-qq-plot.htm - Reference for using Q-Q plot to test for residual normality.