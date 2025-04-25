# Heart Disease Exploratory Data Analysis (EDA)

This repository contains the exploratory data analysis (EDA) for a dataset related to heart disease. The primary goal of this project is to understand the data, identify patterns, and create visualizations that will help to explore the relationship between various factors (such as age, cholesterol levels, etc.) and heart disease presence.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Visualizations](#visualizations)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Overview

This project performs an exploratory data analysis on the heart disease dataset using Python and popular data analysis libraries such as **Pandas**, **Seaborn**, and **Matplotlib**. The purpose of this analysis is to explore key features and provide visual insights into the data, including:

- Distribution of age, cholesterol levels, and other important attributes.
- Relationship between age and heart disease.
- Correlation between various features.
- Visualizing the target distribution (heart disease presence).

## Dataset

The dataset used in this analysis is the **Heart Disease Dataset** (available at [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Heart+Disease)) which contains various medical attributes such as:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Serum cholesterol
- Max heart rate achieved
- Exercise induced angina
- Target: Heart disease presence (1 = Yes, 0 = No)

Make sure the dataset is available in the root directory as `heart.csv`.

## Exploratory Data Analysis

The following steps are included in the EDA process:

1. **Data Structure**: Checking the basic information and structure of the dataset.
2. **Missing Values**: Identifying if any columns have missing values.
3. **Summary Statistics**: Calculating summary statistics such as mean, median, etc.
4. **Visualizations**:
    - Histogram for `age`
    - Boxplot for `chol` (cholesterol levels)
    - Count plot for `target` (heart disease presence)
    - Correlation heatmap
    - Pairplot for selected features and `target`
    - Boxplot for `age` vs. `target`

## Visualizations

The following visualizations are generated and saved to the `heart_eda_outputs` folder:

- **Age Distribution**: A histogram showing the distribution of ages in the dataset.
- **Cholesterol Levels**: A boxplot representing the distribution of cholesterol levels.
- **Heart Disease Presence**: A count plot showing the presence of heart disease (target variable).
- **Correlation Heatmap**: A heatmap showing the correlation between different features.
- **Pairplot**: A pairplot to visualize the relationships between age, cholesterol, max heart rate, and target.
- **Age vs Heart Disease**: A boxplot showing the relationship between age and the presence of heart disease.

## Requirements

To run this project, you need the following Python packages:

- `pandas`
- `matplotlib`
- `seaborn`
- `numpy` (if not already installed with any of the packages above)

## Installation

Clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/heart-disease-eda.git
cd heart-disease-eda
```

Then, create and activate a virtual environment (optional):

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

You can create a `requirements.txt` file with the following dependencies:

```
pandas
matplotlib
seaborn
numpy
```

## Usage

1. Place the `heart.csv` dataset file in the root directory of the project.
2. Run the script `heart_eda.py` to perform the EDA and generate visualizations.

```bash
python heart_eda.py
```

This will create a folder `heart_eda_outputs` and save the plots and summary file in it.

## Results

After running the script, you will get the following output in the `heart_eda_outputs` directory:

- Visualizations:
  - `age_distribution.png`
  - `cholesterol_boxplot.png`
  - `target_distribution.png`
  - `correlation_heatmap.png`
  - `pairplot.png`
  - `age_vs_target.png`
- Summary File:
  - `summary.txt` containing:
    - Data structure
    - Summary statistics
    - Missing values information

