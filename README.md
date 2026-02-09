# Projected-yield-curve-building
This project is based on US treasury data, using datasets that were open source and had sufficient data.

For example the tenors used 2 year, 7 year, 10 year and 30 year had sufficient extractable data, attempts were made to use shorter tenors such as 3 year and 5 year, however the data wasn't available.

This project is meant to aid understanding of future bond and swap yields and show how deep learning architectures can be used to aid that understanding.

```
--- model: LSTM long-short term memory
--- dataset tickers: DGS2, DGS7, DGS10, DGS30, USDSB3L2Y, USDSB3L7Y, USDSB3L10Y, USDSB3L30Y
--- architecture: 64 neurons, droput rate 0.2, dense layer 8 neurons
--- kearning rate: 0.001
--- look back window: 75 days
--- batch size: 32
--- epochs: 50
--- training split: 70% training, data split chronologically to avoid look ahead bias
```
