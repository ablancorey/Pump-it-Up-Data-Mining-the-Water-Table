# Pump it Up: Data Mining the Water Table

This repository contains a machine learning project aimed at predicting faulty water pumps in [Taarifa (Tanzania)](http://taarifa.org). The goal is to help promote access to clean, potable water by leveraging data analysis and predictive modeling techniques.

## Project Overview
This notebook performs a full preprocessing pipeline, analyzing each variable from both an analytical and functional perspective. The key steps include:

- **Data Import & Exploration:** Understanding the dataset, handling missing values, and performing initial visualizations.
- **Feature Engineering:** Creating meaningful features to improve model performance.
- **Model Training & Evaluation:** Implementing and comparing different machine learning models to predict pump functionality.

## Requirements
To run this project, install the necessary dependencies:

```bash
pip install pandas numpy seaborn scikit-learn missingno pandas-profiling
```

## Usage
Run the Jupyter Notebook to preprocess the data and train the models. Adjust hyperparameters and preprocessing techniques as needed to improve performance.

## Dataset
The dataset is provided as part of the [Pump it Up: Data Mining the Water Table](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/) competition. It contains information on thousands of water pumps, including their location, installation year, water quality, and operational status.

## Results & Insights
The analysis provides key insights into the factors influencing pump failure, allowing for better resource allocation in maintaining Tanzania's water infrastructure.

## Model Performance

| Model                     | Score  | Rank  | Programming Language |
|----------------------------|--------|-------|----------------------|
| Random Forest             | 0.8125 | -     | Python               |
| Random Forest (100% data)* | 0.8195 | #2073 | Python               |
| Decision Tree             | 0.7574 | -     | Python               |
| XGBClassifier             | 0.7768 | -     | Python               |

**Note**: The Random Forest (100% data) model was trained using 100% of the available data. This approach is not recommended for real-world scenarios but was useful for achieving a better score in this practice setting.

## Acknowledgments
Thanks to [Driven Data](http://www.drivendata.org) for the dataset and the competition.
