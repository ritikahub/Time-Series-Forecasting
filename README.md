# :chart_with_upwards_trend: Time-Series-Forecasting with Arima and Prophet models: An Introduction
This repository is designed to provide a concise yet comprehensive overview of time series analysis, focusing on key concepts and practical applications. It presents ARIMA models with their variants and Prophet forecasting models, offering a deeper understanding of these powerful tools for time series forecasting.

In the notebook titled **[01-Introduction.ipynb](https://github.com/MKB-Datalab/time-series-analysis-with-SARIMAX-and-Prophet/blob/master/notebooks/01-Intro_time_series_tutorial.ipynb)**, you will gain insights into the characteristics of time series data and discover methods for their identification through a combination of statistical analysis and graphical tools.

Moving forward, in the notebook titled **[02-TimeSeriesForecastingUsingArima.ipynb](https://github.com/MKB-Datalab/time-series-analysis-with-SARIMAX-and-Prophet/blob/master/notebooks/02-Forecasting_with_SARIMAX.ipynb)**, you will be introduced to the world of ARIMA models and their variations. Within this notebook, you will have the opportunity to apply the SARIMA model to a dataset related to store-item sales, which can be accessed [here](https://www.kaggle.com/c/demand-forecasting-kernels-only). The primary objective is to utilize the SARIMA model to make sales forecasts for a future time period, specifically three months ahead.

In the final notebook, **[03-TimeSeriesForecastingUsingFBProphet.ipynb](https://github.com/MKB-Datalab/time-series-analysis-with-SARIMAX-and-Prophet/blob/master/notebooks/03-Forecasting_with_Facebook_Prophet.ipynb)**, we explore the capabilities of Facebook Prophet for time series forecasting. This notebook includes a comprehensive comparison of Prophet with other models, including SARIMAX, as we apply them to the same dataset. The ultimate objective is to assess and contrast the performance of all the models utilized in this analysis, which encompasses both SARIMA and Prophet models.

## Dataset Used

In the practical examples provided within this repository, we utilized the following datasets:

1. **Google Trends Data**: This dataset captures the frequency of searches for the term 'diet' in the United States. It spans from the week starting on `2016-03-27` to the week starting on `2021-03-21`. You can access this data directly from [Google Trends](https://trends.google.com/trends/), and a copy of it is available [here](https://github.com/MKB-Datalab/time-series-analysis-with-SARIMAX-and-Prophet/blob/master/data/raw/time-series/multiTimeline_diet.csv).

2. **Global Temperature Dataset**: This dataset provides global monthly mean temperature anomalies in degrees Celsius, dating back to 1880 and extending to the present. It comprises data from the GISS Surface Temperature (GISTEMP) analysis and the global component of Climate at a Glance (GCAG). The dataset is accessible [here](https://datahub.io/core/global-temp#data), and you can find a copy of it [here](https://github.com/MKB-Datalab/time-series-analysis-with-SARIMAX-and-Prophet/blob/master/data/raw/time-series/monthly_csv.csv).

3. **Kaggle's Store Item Demand Forecasting Challenge Data**: This dataset stems from Kaggle's competition titled the [**Store Item Demand Forecasting Challenge**](https://www.kaggle.com/c/demand-forecasting-kernels-only). It encompasses five years of sales data for various store items, partitioned into a training dataset (train.csv) and a test dataset (test.csv). Specifically, our examples drew from a subset of this data, which can be located [here](https://github.com/MKB-Datalab/time-series-analysis-with-SARIMAX-and-Prophet/blob/master/data/processed/sales_store_2_item_28.csv).

These datasets were employed in practical demonstrations and analyses throughout the repository to illustrate various time series forecasting techniques and concepts.

## Tools

Certainly! Here's a brief description of the tools used in this repository:

1. **statsmodels**:
   - **Description**: statsmodels is a Python library that provides classes and functions for the estimation of many different statistical models, as well as for conducting statistical tests and exploring data.
   - **Usage**: In the context of time series analysis, statsmodels is often used for implementing models like ARIMA (AutoRegressive Integrated Moving Average) and SARIMA (Seasonal ARIMA). It offers a wide range of statistical tests and tools for model diagnostics and parameter estimation.
   
2. **Prophet**:
   - **Description**: Prophet is an open-source forecasting tool developed by Facebook. It is designed for forecasting time series data that exhibits seasonality and trends. Prophet is particularly useful for business and financial forecasting, where data may have irregularities and missing values.
   - **Usage**: Prophet simplifies the forecasting process by automatically handling aspects like seasonality, holidays, and outliers. It provides a straightforward interface for time series forecasting and is known for its ability to produce accurate forecasts with minimal manual configuration.

These tools are essential for performing various time series forecasting tasks and are commonly used in data science and statistical analysis to model and predict time-dependent data patterns. In the repository, you'll find practical examples demonstrating how to use these tools for time series analysis and forecasting.

## Installing Requirements

* Install requirements using `pip install -r time_series_requirements.txt`.
  * Make sure you use Python 3.
  * You may want to use a virtual environment for this.

To set up the necessary dependencies for this repository, follow these steps:

1. Ensure you are using Python 3 for this installation.
2. It is recommended to create and activate a virtual environment to keep your project isolated. You can create one using `virtualenv` or `conda`, depending on your preference.

   **Using virtualenv:**
   
   ```bash
   # Install virtualenv if you haven't already
   pip install virtualenv
   
   # Create a virtual environment (replace 'venv' with your preferred name)
   virtualenv venv
   
   # Activate the virtual environment
   source venv/bin/activate  # On Windows, use 'venv\Scripts\activate'
   ```

   **Using conda:**
   
   ```bash
   # Create a conda environment (replace 'env_name' with your preferred name)
   conda create --name env_name python=3
   
   # Activate the conda environment
   conda activate env_name
   ```

3. Once your virtual environment is active, navigate to the root directory of the repository where `time_series_requirements.txt` is located.

4. Install the required packages using `pip`:

   ```bash
   pip install -r time_series_requirements.txt
   ```

5. This will install all the necessary packages and dependencies specified in the `time_series_requirements.txt` file.

Now you have the required environment set up with the needed packages installed for working with the repository's code and examples.
