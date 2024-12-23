

The goal of this assignment is to fetch live cryptocurrency data for the top 50 cryptocurrencies, analyse it, and present the data in a live-updating Excel sheet.
Libraries 
•	requests: Fetch data from the CoinGecko API.
•	pandas: Manipulate and analyze the data.
•	openpyxl: Write the processed data to an Excel file.
•	time: Control the interval between data updates (every 5 minutes)
Data Collection: In order to fetch the live data I used , the CoinGecko API . Every five minutes, a query was made to the API to retrieve new data, which was subsequently processed and stored in an Excel document. Each cryptocurrency's name, symbol, market capitalization, trading volume, and 24-hour price change are all included in the statistics.

•	vs_currency: Specifies that data should be in USD.
•	order: Ensures the data is ordered by market capitalization in descending order.
•	per_page: Fetches 50 cryptocurrencies.
•	page: Requests the first page, containing the top 50 cryptocurrencies.
Data Analysis:
•	The top five cryptocurrencies were analysed by looking at their market capitalization.
•	Average Price: The average cost of the top 50 cryptocurrencies was determined.
•	Analysis of Price Change: The largest and lowest 24-hour percentage price fluctuations were analysed.
Excel file Generation-:The data was saved in an Excel file named crypto_data.xlsx, with live updates every 5 minutes.
•	Used of pandas and openpyxl to write the data to an Excel file
•	Data Fetching: The CoinGecko API is used to retrieve cryptocurrency data every five minutes.
•	Writing to Excel: The update_excel function overwrites any existing information in an Excel file (crypto_data.xlsx) with the updated data after it has been retrieved.
•	Repeating the Process: The while True loop and the time let the process to repeat indefinitely, fetching and writing new data to the Excel file every five minutes, delay in sleep (300).



 



 
