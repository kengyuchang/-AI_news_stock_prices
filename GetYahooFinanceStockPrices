# Import necessary libraries
import pandas as pd
import yfinance as yf
import datetime

# Function to fetch Apple stock prices from Yahoo Finance
def fetch_stock_data(ticker, start_date, end_date):
    stock_data = yf.download(ticker, start=start_date, end=end_date)
    return stock_data

# Define date range and fetch data
start_date = datetime.datetime(2023, 1, 1)
end_date = datetime.datetime(2024, 12, 31)

# Fetch Apple stock data
apple_stock = fetch_stock_data("AAPL", start_date, end_date)
apple_stock.reset_index(inplace=True)

# Save data to CSV file
apple_stock.to_csv("apple_stock_data.csv", index=False)

print("Data fetching completed! Stock data is saved.")
