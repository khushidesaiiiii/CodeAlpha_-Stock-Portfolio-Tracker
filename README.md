Here’s a polished `README.md` file for the stock portfolio manager code you shared:

---

# Stock Portfolio Manager

This is a **simple Python console application** that allows users to manage a stock portfolio.  
It uses real-time stock data from the **Alpha Vantage API** to calculate the current value of the portfolio.

---

## Features

- 📈 Add stocks to your portfolio.
- 📉 Remove stocks from your portfolio.
- 💰 View the total current value of your portfolio based on live market prices.
- 🔄 Automatically fetches real-time stock data using the Alpha Vantage API.

---

## Requirements

- Python 3.x
- `requests` library

Install dependencies using:
```bash
pip install requests
```

---

## Setup

1. **Get an API Key**  
   - Sign up at [Alpha Vantage](https://www.alphavantage.co/support/#api-key) to get a free API key.

2. **Update the API Key**  
   - Replace the placeholder API key in the code:
     ```python
     API_KEY = 'FK75ZJ9M9N8UUZOI'
     ```
   - with your actual key.

---

## How to Run

```bash
python portfolio_manager.py
```

Follow the on-screen menu to:

- **1.** Add stocks (provide symbol and quantity).
- **2.** Remove stocks.
- **3.** View your portfolio’s real-time value.
- **4.** Exit the program.

---

## Code Structure

- `get_stock_data(symbol)`: Fetches the latest price and change percentage for a given stock symbol.
- `Portfolio` class:
  - `add_stock(symbol, quantity)`: Adds stock to the portfolio.
  - `remove_stock(symbol, quantity)`: Removes stock from the portfolio.
  - `get_portfolio_value()`: Calculates the total value of all holdings.
- `main()`: Runs the menu-driven application.

---

## Example

```
1. Add the stock to portfolio
2. Remove the stock from portfolio
3. View the portfolio value
4. Exit

Enter your choice: 1
Enter the stock symbol: AAPL
Enter the quantity: 5

Enter your choice: 3
Portfolio value: $845.50
```

---

## Notes

- Make sure you have a stable internet connection to fetch real-time stock data.
- Be cautious about API rate limits (Alpha Vantage allows 5 API calls per minute for free accounts).
- The application does not store your portfolio data after exiting — it runs entirely in-memory.

---
