# NBA Shot Selection Prediction 

This project focuses on analyzing and predicting NBA shot selections, specifically leveraging historical shot data from Kobe Bryant's career. Using data science and machine learning techniques, the goal is to predict whether a given shot was made (`1.0`) or missed (`0.0`) based on features like shot location, distance, and time remaining.

##  Project Overview
* **Objective:** Predict the `shot_made_flag` for missing test records.
* **Dataset:** Contains over 30,000 shot records with detailed spatial (latitude/longitude) and temporal attributes.
* **Status:** Exploration & Data Preparation Phase.

---

## Project Structure
```text
├── NBA SHOT SELECTION.ipynb   # Main Jupyter Notebook containing the analysis
├── data/
│   └── data.csv               # The raw NBA shot selection dataset
└── README.md                  # Project documentation

 Dataset Features
The dataset (data.csv) splits into a training set and a prediction set based on the shot_made_flag column.

Training rows: 25,697 (Contains labels)

Prediction rows: 5,000 (Missing labels—to be predicted)

Key Columns Highlighted in Analysis:
lon / lat: Longitude and latitude coordinates of the shot taken on the court.

shot_made_flag: The target variable (1 for a basket, 0 for a miss).

🚀 Getting Started
1. Prerequisites
Make sure you have a Python environment (like Anaconda) installed with the following libraries:

pandas

numpy

matplotlib

seaborn

scikit-learn

2. Setup & Installation
Clone or download this repository to your local machine.

Place your CSV data file inside a data/ folder (or update the path in the notebook to match your local setup).

Open your terminal or Anaconda prompt and launch JupyterLab:

Bash
jupyter lab
Open NBA SHOT SELECTION.ipynb and run the cells sequentially.

 Current Progress
 Shot Visualization (Shot Map)
A scatter plot mapping the coordinates (lon, lat) with transparency handling (alpha=0.1) is utilized to visually isolate high-density shot selection areas on the court.

🛠️ Data Preparation
Successfully separated the dataset into train_data (where shot_made_flag is known) and test_data (where shot_made_flag is null) to prepare for model training.

Next Phase: Feature selection, encoding categorical text features, and model training.