![logo](docs/source/_static/pics/title.PNG)

Robin-Stocks API Library
========================
This library provides a pure python interface to interact with the Robinhood API, Gemini API,
and TD Ameritrade API. The code is simple to use, easy to understand, and easy to modify.
With this library you can view information on stocks, options, and crypto-currencies in real time, 
create your own robo-investor or trading algorithm, and improve your programming skills.

Installing
========================

```
git clone https://github.com/peter777-cloud/robin_stocks.git
```
```
cd robin_stocks
```

Now that you have cd into the repository you can type

```
pip install .
```

Supported APIs
==============
The supported APIs are Robinhood, Gemini, and TD Ameritrade. For more information about how to use the different APIs, visit the README
documents for `Robinhood Documentation`_, `Gemini Documentation`_, and `TDA Documentation`_.

Below are examples on how to call each of those modules.

```
import robin_stocks.robinhood as rh
```
```
import robin_stocks.gemini as gem
```
```
import robin_stocks.tda as tda
```

# Here are some example calls

```
gem.get_pubticker("btcusd") # gets ticker information for Bitcoin from Gemini
```
```
rh.get_all_open_crypto_orders() # gets all cypto orders from Robinhood
```
```
tda.get_price_history("tsla") # get price history from TD Ameritrade 
```



# List of Functions and Example Usage
===================================

If you would like to see some example code and instructions on how to set up two-factor authorization for Robinhood,
go to the [Robinhood Documentation](Robinhood.rst).

For detailed instructions on how to generate API keys for TD Ameritrade and how to use the API, go to the [TDA Documentation](tda.rst).

For detailed instructions on how to generate API keys for Gemini and how to use both the private and public API, go to the [Gemini Documentation](gemini.rst).
