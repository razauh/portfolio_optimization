# Portfolio Performance Enhancement Using Random Forest

This repository contains the implementation of the research paper titled "Enhancing Portfolio Performance: A Random Forest Approach to Volatility Prediction and Optimization" by Vedant Rathi, Meghana Kshirsagar, and Conor Ryan. The study explores the application of Random Forest in optimizing portfolio performance by predicting volatility and maximizing the Sharpe Ratio.

## Overview

The implementation focuses on three main aspects:
1. **Volatility Prediction**: Utilizes Random Forest models to predict portfolio volatility based on historical data of various financial instruments.
2. **Portfolio Optimization**: Employs optimization techniques to maximize the Sharpe Ratio, balancing the return against volatility.
3. **Data Handling**: Handles real-world financial data fetched using the `yfinance` API to model and predict future performance.

## Implementation Details

### Data Retrieval
- Historical data for the tickers `VTSAX`, `VTIAX`, `VBTLX`, `VDE`, `VGSLX`, `OPGSX`, and `BTC-USD` are downloaded for the period from 2015 to 2023 using Yahoo Finance.

### Volatility Prediction
- The Random Forest algorithm is applied to predict the volatility of portfolios composed of the mentioned financial instruments.
- The dataset is split into training and testing subsets, with 80% used for training the Random Forest models.

### Portfolio Optimization
- The portfolio optimization is achieved by maximizing the Sharpe Ratio using the `scipy.optimize` library. This involves calculating expected returns, portfolio volatility, and subsequently the Sharpe Ratio under various constraints.

### Results
The implementation achieved the following results:
- **Classifier Accuracy**: 0.92
- **Regressor Mean Squared Error**: 7.751834721707441e-05
- **Regressor R-squared Value**: 0.9652789905605766
- **Optimized Weights**: `[0.14285714, 0.14285714, 0.14285714, 0.14285714, 0.14285714, 0.14285714, 0.14285714]`
- **Expected Portfolio Return**: 0.08142857142873532
- **Expected Portfolio Volatility**: 0.6517280821266038
- **Sharpe Ratio**: 0.09425490954493239


## Contributions

Contributions to this project are welcome. You can enhance the model's predictive accuracy, optimize the code, or improve the data preprocessing steps.

## License

This project is open-sourced under the MIT license.

## Acknowledgements

The implementation is based on the research **Enhancing Portfolio Performance: A Random Forest Approach to Volatility Prediction and Optimization**
conducted by **Vedant Rathi, Meghana Kshirsagar, and Conor Ryan from the University of Limerick, Ireland**. Their insights into using machine learning for financial optimizations have been invaluable.

