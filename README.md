# GoldCapstone
# Gold Price Analysis

This project analyzes historical gold price data to identify trends, patterns, and relationships with other financial indicators. The analysis leverages Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn for data manipulation, analysis, and visualization.

## Project Overview

The project aims to understand the dynamics of gold prices and their potential correlations with other market variables. This is achieved through a systematic process of data loading, exploration, cleaning, analysis, and visualization. Key features of the project include:

- **Data Loading:** Loading historical gold price data from a CSV file into a Pandas DataFrame.
- **Data Exploration:** Exploring data characteristics such as shape, data types, summary statistics, distribution, missing values, and potential outliers.
- **Data Cleaning:** Handling incorrect data types, addressing potential outliers, and imputing missing values.
- **Data Analysis:** Identifying trends and patterns in gold prices and calculating key statistics.
- **Feature Engineering:** Creating new features such as moving averages and rolling standard deviations.
- **Data Visualization:** Generating informative visualizations of gold price trends and relationships with other variables.

## Business Questions

The project seeks to answer specific business questions, including:

- What is the average gold price (GLD) over the observed period?
- Is there a correlation between the gold price (GLD) and the S&P 500 index (SPX)?

## Key Findings

The analysis reveals valuable insights into gold price dynamics and correlations. Key findings include:

## Summary:

### 1. Q&A

* **What is the average gold price (GLD) over the observed period?** The average gold price is approximately 121.18.
* **Is there a correlation between the gold price (GLD) and the S&P 500 index (SPX)?**  The correlation coefficient between GLD and SPX is approximately 0.09, indicating a weak correlation.


### 2. Data Analysis Key Findings

* **Data Cleaning:** 25 rows (outliers) were removed from the dataset based on the IQR method applied to the 'GLD' column. All relevant columns ('SPX', 'GLD', 'USO', 'SLV', 'EUR/USD') were converted to numeric (`float64`) data type. No missing values were found after cleaning.
* **Correlation Analysis:** A weak positive correlation (approximately 0.09) was observed between gold prices (GLD) and the S&P 500 index (SPX).
* **Feature Engineering:** New features were engineered, including 7-day moving averages for 'GLD' and 'SPX' (GLD_MA7, SPX_MA7), 7-day rolling standard deviations (GLD_STD7, SPX_STD7), and percentage changes (GLD_PCT_CHANGE, SPX_PCT_CHANGE) for 'GLD' and 'SPX'.

### 3. Insights or Next Steps

* **Investigate other potential correlations:** While the correlation between GLD and SPX was weak, exploring relationships with other variables like 'USO', 'SLV', and 'EUR/USD' may reveal more significant connections.  Further analysis of the correlation matrix and other bivariate visualizations could yield insights.
* **Explore time-series modeling:** Given the time-series nature of the data, time-series models (e.g., ARIMA, Prophet) could be used to forecast future gold prices and further analyze the trends observed in the visualizations, particularly after adding the engineered features.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Usage

1. Clone the repository: `[git clone [repository URL]](https://github.com/lukedaduke2789/GoldCapstone)`
2. Install required libraries: `pip install pandas numpy matplotlib seaborn`
3. Run the Jupyter Notebook: `jupyter notebook gold_price_analysis.ipynb`

## Contributing

Contributions to this project are welcome. Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your forked repository.
5. Submit a pull request to the original repository.

## License

This project is licensed under some kind of license
