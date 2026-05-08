# Food Delivery Time Prediction Analysis

## Project Overview
This project focuses on analyzing and preprocessing a real-world food delivery dataset to understand the key factors affecting food delivery time. The project was developed using Python for data cleaning, preprocessing, descriptive analysis, statistical analysis, and data visualization.

The main objective of this project is to prepare a clean and structured dataset suitable for future machine learning prediction models.

---

## Project Objectives
- Load and explore the food delivery dataset
- Clean and preprocess raw data
- Handle missing values and incorrect data types
- Remove outliers using the IQR method
- Encode categorical variables
- Perform descriptive statistical analysis
- Conduct hypothesis testing
- Visualize important delivery patterns
- Prepare the dataset for future predictive modelling

---

## Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

---

## Project Structure

```text
food-delivery-time-prediction/
│
├── data/
│   └── train.csv
│
├── notebook/
│   └── food-delivery-time-prediction.ipynb
│
├── outputs/
│   ├── charts/
│   ├── cleaned_delivery_dataset1.csv
│   └── food-delivery-time-prediction.html
│
└── README.md
```

---

## Dataset Information

The dataset contains delivery-related information such as:

- Delivery person age
- Delivery person ratings
- Weather conditions
- Traffic density
- City type
- Festival information
- Order time and date
- Delivery time

### Target Variable
`Time_taken_min`

This variable represents the total time taken to deliver the food and is used as the main analysis target.

---

## Data Cleaning and Preprocessing

### Handling Data Types
- Converted incorrect columns into appropriate numeric formats
- Cleaned `Time_taken(min)` column
- Converted date and time fields into usable formats

### Handling Missing Values
- Replaced missing values using median values
- Removed invalid records

### Feature Engineering
Created additional useful features such as:
- Order hour
- Order day
- Delivery time difference

### Outlier Removal
- Used the Interquartile Range (IQR) method
- Removed extreme delivery time values

### Encoding
- Applied One-Hot Encoding to categorical variables

---

## Final Dataset Summary

| Metric | Value |
|---|---|
| Original Records | 45,593 |
| Records After Cleaning | 43,607 |
| Original Features | 20 |
| Features After Preprocessing | 30 |
| Missing Values Remaining | 0 |
| Outlier Rows Removed | 1,986 |

---

## Key Findings

### Traffic Density

| Traffic Level | Mean Delivery Time |
|---|---|
| Low | 21.28 min |
| Medium | 26.72 min |
| High | 27.07 min |
| Jam | 30.78 min |

### Festival Impact

| Festival | Mean Delivery Time |
|---|---|
| Yes | 44.61 min |
| No | 25.81 min |

### Weather Conditions
- Foggy weather resulted in the highest average delivery time
- Sunny weather showed the lowest delivery time

### Ratings vs Delivery Time
Higher-rated delivery personnel generally completed deliveries faster.

---

## Statistical Analysis Performed
- One-Way ANOVA
- Independent Samples T-Test
- Pearson Correlation Analysis

---

## Visualizations Included
The project contains multiple visualizations including:

- Histograms
- Boxplots
- Pie Charts
- Bar Charts
- Scatter Plots
- Correlation Heatmaps
- Line Charts

All generated charts are stored inside:

```text
outputs/charts/
```

---

## Output Files

| File | Description |
|---|---|
| `cleaned_delivery_dataset1.csv` | Final cleaned dataset |
| `food-delivery-time-prediction.html` | Exported notebook/report |
| `food-delivery-time-prediction.ipynb` | Main Jupyter notebook |

---

## How to Run the Project

### Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

### Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
food-delivery-time-prediction.ipynb
```

---

## Future Improvements
- Build machine learning prediction models
- Add distance-based delivery analysis
- Develop dashboard visualizations
- Deploy prediction system as a web application

---

## Author
S. Akshan  
BSc in Data Science  
NSBM Green University