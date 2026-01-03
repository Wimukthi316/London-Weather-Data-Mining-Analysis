# 📊 London Weather Analysis - Data Mining Project

A comprehensive data mining project focused on analyzing London weather patterns using clustering and classification techniques. This project demonstrates the complete data mining pipeline from data preparation to model evaluation.

## 🎯 Project Overview

This project analyzes London weather data to identify seasonal patterns and classify weather conditions. It implements both unsupervised (K-Means clustering) and supervised (Decision Tree classification) machine learning algorithms from scratch, along with extensive data preparation and visualization.

## 📁 Project Structure

```
Data Mining Assignment/
│
├── London_Weather_Analysis.ipynb        # Main Jupyter notebook with complete analysis
├── london_weather_with_class_labels.csv # Dataset with weather measurements
├── Coursework_1_DataMining_T.html       # HTML export of the analysis
└── README.md                            # Project documentation
```

## 🔍 Features & Tasks

### Task 1: Data Preparation
- **Data Loading & Exploration**: Initial dataset analysis with 459 instances and multiple weather features
- **Data Cleaning**: Handling missing values, removing empty columns, and type conversions
- **Numerosity Reduction**: Stratified sampling to reduce dataset to 60% (275 instances) while maintaining class distribution
- **Feature Reduction**: Correlation-based selection of top 3 features (mean_temp, max_temp, min_temp)

### Task 2: Clustering Analysis (K-Means)
- **Custom K-Means Implementation**: Built from scratch for 3D data
- **Optimal K Selection**: Elbow method using Within-Cluster Sum of Squares (WCSS)
- **Multiple Runs**: 3 iterations with different random seeds for consistency validation
- **3D Visualization**: Interactive scatter plots showing cluster assignments
- **Evaluation Metrics**: Silhouette Score and Davies-Bouldin Index

### Task 3: Classification (Decision Tree)
- **Custom Decision Tree**: ID3-inspired algorithm implemented from scratch
- **Discretization**: Continuous features converted to categorical using quartile-based binning
- **Train-Test Split**: 80-20 stratified split for robust evaluation
- **Performance Metrics**: Accuracy, Precision, Recall, F1-Score, and Confusion Matrix
- **Visualization**: Decision tree structure and performance metrics plots

## 🛠️ Technologies Used

- **Python 3.x**
- **Libraries**:
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computing
  - `matplotlib` - Data visualization
  - `seaborn` - Statistical data visualization
  - `scikit-learn` - Data preprocessing and evaluation metrics

## 📊 Dataset

The dataset (`london_weather_with_class_labels.csv`) contains weather measurements from London with the following features:

- **Date**: Timestamp of measurements
- **Mean Temperature**: Average temperature
- **Max Temperature**: Maximum temperature
- **Min Temperature**: Minimum temperature
- **Cloud Cover**: Cloud coverage percentage
- **Humidity**: Humidity levels
- **Precipitation**: Rainfall amount
- **Pressure**: Atmospheric pressure
- **Sunshine**: Hours of sunshine
- **Global Radiation**: Solar radiation levels
- **Class**: Month labels (01-12)

## 🚀 Getting Started

### Prerequisites

```bash
# Install required packages
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Running the Analysis

1. Clone the repository:
```bash
git clone <repository-url>
cd "Data Mining Assignment"
```

2. Open the Jupyter notebook:
```bash
jupyter notebook London_Weather_Analysis.ipynb
```

3. Run all cells to execute the complete analysis pipeline

## 📈 Key Results

### Clustering Results
- **Optimal K**: 4 clusters (representing seasonal patterns)
- **Silhouette Score**: ~0.45-0.50 (moderate cluster separation)
- **Convergence**: Typically 10-20 iterations

### Classification Results
- **Accuracy**: 85-90% on test set
- **Model Depth**: 5-7 levels
- **Feature Importance**: Temperature features most discriminative

## 🔬 Methodology

### Data Reduction Approach
1. **Numerosity Reduction**: Stratified sampling maintains class balance while reducing computational complexity
2. **Feature Selection**: Correlation analysis identifies temperature features as most predictive
3. **Normalization**: StandardScaler applied for distance-based algorithms

### Algorithm Implementations
- **K-Means**: Euclidean distance, random initialization, iterative refinement
- **Decision Tree**: Information gain-based splitting, entropy calculation, depth limiting

## 📝 Project Highlights

- ✅ All algorithms implemented from scratch (not using sklearn.cluster or sklearn.tree)
- ✅ Comprehensive data preprocessing and feature engineering
- ✅ Multiple evaluation metrics for robust performance assessment
- ✅ Clear visualizations for data exploration and results presentation
- ✅ Detailed justifications for methodological choices
- ✅ Professional documentation and code organization

## 🎓 Academic Context

This project was completed as part of a Data Mining coursework assignment, demonstrating:
- Understanding of fundamental data mining concepts
- Ability to implement ML algorithms from first principles
- Skills in data preprocessing and feature engineering
- Proficiency in Python and data science libraries
- Critical analysis and interpretation of results
