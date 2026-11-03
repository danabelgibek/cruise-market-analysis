# Cruise Market Analysis

## Project Overview

This project explores cruise market data collected from the Center Cruises website. The goal was to collect, clean, transform, and analyze cruise offers to understand pricing patterns and differences across cruise companies, destinations, regions, and seasons.

The project demonstrates an end-to-end data analytics workflow, from web scraping to exploratory data analysis and visualization.

## Objectives

- Collect cruise offer data using web scraping.
- Clean and preprocess raw data.
- Explore pricing patterns across companies and regions.
- Analyze seasonal differences in cruise prices.
- Create additional features for deeper analysis.
- Visualize findings using statistical and interactive charts.

## Tools & Technologies

- **Python** — main programming language
- **Pandas & NumPy** — data cleaning and manipulation
- **Requests & BeautifulSoup** — web scraping
- **Matplotlib & Seaborn** — data visualization
- **Plotly** — interactive visualizations
- **Scikit-learn** — feature encoding and scaling
- **SciPy** — statistical analysis

## Project Workflow

### 1. Data Collection
Collected cruise offer information from the Center Cruises website using Requests and BeautifulSoup.

The initial dataset contained approximately 20,000 records.

### 2. Data Cleaning & Preprocessing
- Checked missing values and duplicate records.
- Removed duplicate entries.
- Converted price and duration columns into numeric formats.
- Processed departure and return dates.
- Translated text fields into English.
- Prepared the dataset for further analysis.

### 3. Feature Engineering
Created additional variables, including:
- Price per night
- Price segments (Budget, Mid-range, Luxury)
- Departure month and day of the week
- Season
- Number of ports
- Geographic region
- Company and ship-related features

### 4. Exploratory Data Analysis
Analyzed:
- Average cruise prices by region.
- Pricing differences between cruise companies.
- Price distribution and price segments.
- Seasonal and monthly pricing patterns.
- Relationships between numerical variables.
- The most and least expensive cruise offers per night.

### 5. Data Visualization
Created static and interactive visualizations, including:
- Correlation heatmaps.
- Seasonal price distribution boxplots.
- Monthly pricing trend charts.
- Company comparison charts.
- Regional market composition charts.
- Interactive maps and grouped bar charts.

## Dataset Summary

| Metric | Value |
|---|---:|
| Initial records | 20,000 |
| Duplicate records detected | 11,457 |
| Records in final EDA dataset | 5,306 |
| Features in final EDA dataset | 47 |

## Key Analytical Areas

The analysis explores how cruise pricing varies by company, region, season, and trip duration.

It also examines differences between average and median prices and investigates monthly pricing patterns.

## Repository Structure

- `arbuz.ipynb` — original Jupyter Notebook containing the analysis.

## How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Open the notebook in Jupyter Notebook or Google Colab.
4. Run the notebook cells in order.

```bash
pip install pandas numpy requests beautifulsoup4 matplotlib seaborn plotly scikit-learn scipy deep-translator
```

**Note:** The original data collection step retrieves information from the source website. Website structure and availability may change, so scraping may require adjustments. The notebook also uses intermediate CSV files created during preprocessing.

## Limitations

- The dataset represents collected website offers rather than the entire cruise market.
- Regional classifications are based on keyword matching.
- Price values and currency should be verified against the original source before making financial comparisons.
- The analysis is descriptive and does not establish causal relationships.

## Author

**Dana Belgibek**

Data Science Student | SDU University

[GitHub Profile](https://github.com/danabelgibek)
