# JPMC Task 1
Starter repo for task 1 of the JPMC software engineering program
# Trader's Dashboard Enhancement: Stock Correlation Monitoring

## Overview

This project aims to enhance a trader's dashboard by adding a chart that allows the identification of under/over-valued stocks. The trader will be able to monitor two historically correlated stocks and visualize when the correlation between the two weakens. Such instances may signal a potential trade strategy: simultaneously buying the relatively underperforming stock and selling the relatively outperforming stock. If the two prices subsequently converge, the trade should be profitable.

## Technologies Used

- **Python 3**: The primary programming language for this project. Ensure you have a recent version installed.
- **Perspective**: JPMorgan Chase's open-source data visualization software, used for interactive charts.
- **yfinance**: Python library for fetching historical stock data from Yahoo Finance.
- **pandas**: Data manipulation library for handling and analyzing stock data.
- **matplotlib**: Plotting library for additional visualizations.
- **requests**: Library for making HTTP requests to data feeds.

## Set-Up

Before you can tackle any software development task, you need to set up your development environment. You can think of your local development environment as a virtual workbench with all the tools necessary to work on your project. To set up your dev environment, follow these instructions:

1. **Install Python 3**:
   - Ensure Python 3 is installed on your system. Any recent version will work, but the most up-to-date version is advisable.
   - For installation instructions, check out this guide from Real Python: [Installing Python](https://realpython.com/installing-python/).

2. **Fork and Clone the Starter Repo**:
   - Fork the repository from GitHub: [Fork Repository](https://github.com/theforage/forage-jpmc-swe-task-1).
   - IMPORTANT: Uncheck the “Copy the main branch only” box in the fork dialog. A model answer is provided in a separate branch from `main`.
   - Clone the forked repository to your local machine:
     ```bash
     git clone https://github.com/<your-username>/forage-jpmc-swe-task-1.git
     cd forage-jpmc-swe-task-1
     ```

3. **Open the Project in Your IDE**:
   - Open the project in your IDE of choice. If you don't have a preferred Python IDE, consider [PyCharm Community Edition](https://www.jetbrains.com/pycharm/download/) by JetBrains. It's powerful, feature-rich, and free.

4. **Create a Virtual Environment**:
   - Create a new virtual environment in the project root. In PyCharm, you can do this using the “Configure Python Interpreter” option in settings. Alternatively, use the terminal:
     ```bash
     python -m venv venv
     source venv/bin/activate  # On Windows use: venv\Scripts\activate
     ```

5. **Install Project Dependencies**:
   - Install all required dependencies listed in the `requirements.txt` file:
     ```bash
     pip install -r requirements.txt
     ``` 

## Implementation Steps

1. **Interface with Financial Data Feed**:
   - Connect to the relevant financial data feed.
   - Retrieve and process the data for the two stocks being monitored.

2. **Calculate Historical Correlation**:
   - Compute the rolling correlation between the two stocks.
   - Identify when the correlation weakens beyond a specified threshold.

3. **Visualize the Data**:
   - Use Perspective to create an interactive chart.
   - Highlight instances where the stocks deviate from their historical correlation, signaling potential trade opportunities.

## Resources

- **Perspective Documentation:** [Perspective GitHub Repository](https://github.com/finos/perspective)
- **Financial Data Feed API:** Access a reliable financial data API such as Alpha Vantage, Yahoo Finance, or another service offering historical stock data.

