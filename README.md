# Google Play Store Exploratory Data Analysis

## Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on the Google Play Store dataset, covering approximately 10,000 apps. It focuses on data cleaning, statistical summaries, and visualizations to reveal patterns in app categories, ratings, installs, reviews, pricing, sizes, and content ratings.[1]

The analysis demonstrates practical data science workflow: from raw data ingestion to actionable insights for app developers and marketers.

## Dataset
The dataset is a standard Kaggle-sourced Google Play Store collection with 13 columns:
- App name, category, ratings, reviews
- Installs, size, price, content rating
- Genres, last updated, current version, Android version

Common issues addressed include inconsistent install formats ("1M+"), price strings ("$4.99"), missing ratings, and size variations ("Varies with device").[2][3]

## Methodology
Standard EDA pipeline implemented in Jupyter Notebook:
- **Data Loading & Inspection**: Shape, info, describe, null checks
- **Cleaning**: Remove duplicates, parse installs/prices/sizes to numerics, handle NaNs
- **Univariate Analysis**: Distributions of ratings, installs, categories
- **Bivariate/Multivariate**: Correlations (reviews vs ratings), category comparisons
- **Visualizations**: Histograms, boxplots, heatmaps, bar charts via Matplotlib/Seaborn

## Key Insights
- **Games** category leads in total installs, followed by **Tools** and **Entertainment**
- Strong correlation between review count and ratings (r ≈ 0.6-0.7 typical)
- Free apps (~92%) dominate; paid apps average lower installs
- "Everyone" content rating correlates with higher adoption and ratings
- Smaller app sizes (<20MB) show better install rates

These findings highlight optimization opportunities like targeting high-install categories and minimizing size.[4][1][2]

## Tech Stack
Built with standard data analysis tools:
- Python 3.x
- Pandas & NumPy for data cleaning and wrangling
- Matplotlib & Seaborn for charts and visualizations
- Jupyter Notebook for the interactive analysis

## Repository Contents
```
playstore_eda.ipynb     # Full analysis walkthrough
googleplaystore.csv     # Raw dataset (~10K apps)
README.md              # You're reading it!
```

Open the notebook directly on GitHub or in Jupyter for interactive exploration
