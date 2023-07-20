Automated Trading using Python
Description
Automated Trading using Python is a data science project that implements an automated trading system. The code provided fetches financial data from Quandl API for a specific stock, calculates daily returns, and generates a 50-day moving average. The project aims to assist traders in making informed decisions based on historical data and technical indicators.

Installation
Ensure you have Python 3.x installed on your system.
Install the required libraries using the following command:
bash
Copy code
pip install pandas quandl numpy matplotlib
Set up a Quandl API key by signing up at https://www.quandl.com/.
Usage
Replace <API KEY> with your Quandl API key in the code.
Run the provided code to fetch stock data, calculate daily returns, and generate the 50-day moving average.
python
Copy code
import pandas as pd
import quandl as qd
import numpy as np
import matplotlib.pyplot as plt

qd.ApiConfig.api_key = "<API KEY>"
msft_data = qd.get("XSHE/200413", start_date="2010-01-01", end_date="2018-01-01")

# ... rest of the code ...

plt.show()
Contributing
Contributions to this project are welcome. Feel free to submit bug reports, feature requests, or improvements through pull requests.
