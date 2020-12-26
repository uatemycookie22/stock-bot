# StockBot

Author: Ryan Cullen

StockBot is a Python script for designing and testing your own daily stock trading algorithms.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install matplotlib and yfinance from your command line.

```bash
pip install matplotlib
pip install yfinance
```

## Usage
You will be asked to enter a ticker for the stock that you want to test the algorithm on.

If you want to modify the algorithm and design your own, you only need to change the Decide() method. That method takes three functions, and you can decide what those are or design your own inputs. My implementation uses moving averages and their derivatives/concavity (the class for which is set up for you to use in your own algorithm).

Entering 'today' as the ticker will show you a list of the latest hypothetical orders from a currently limited watchlist ('BABA', 'IBM', 'PEN', 'GOOG', 'SPCE', 'AMD', 'NIO', 'ARKG', 'PENN', 'MRNA', 'WMT', 'AAPL', 'SBUX', 'NKE', 'SNE') while also showing the date of the order, the current performance of the portfolio, and the average performance. These orders are from a hypothetical portfolio that ran based on the algorithm's decisions starting from 1 year before you use the program. This can be potentially problematic as the performance statistics can start being misleading from a past event (e.g. if you run the 'today' command on March 20th 2021, the algorithm will start in March 20th 2020 when the market experienced a dramatic recession and showing an absurdly high performance).
## Roadmap
The goal for this script is of course for it to be as robust and generalized as possible. To do this, one idea is to use Reinforcement Learning to fine tune the thresholds on the fly. If you have experience with ML or deep learning I very much encourage you to make conributions!!


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.


