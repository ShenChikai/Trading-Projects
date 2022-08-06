# MACD
## This part of the project implements calcualtion of MACD along with its sub-associated indicators, like EMA, Signal Line, and Gap b/w MACD and Signal in the form of a histogram.
## Belows concepts and formulas are from source: https://www.investopedia.com/

> ## **EMA** <br>
> Exponential Moving Average, unlike Simple Moving Average (SMA), is a moving average (MA) that places a greater weight and significance on the most recent data points. Traders often use several different EMA lengths, such as 10-day, 50-day, and 200-day moving averages.
> 
> Formula:
> $$EMA_{Today} = Close_{Today} \cdot Multiplier + EMA_{yesterday} \cdot (1-Multiplier)$$
> $$Multiplier = \frac{Smoothing}{1 + Days}$$
>
> *The initial EMA will be a SMA (I use the close price for this project)* <br>
> *Common choice for Smoothing = 2 gives the most recent observation more weight.* <br>
> *If the smoothing factor is increased, more recent observations have more influence on the EMA.*

> ## **MACD** <br>
> Moving average convergence divergence (MACD) is a trend-following momentum indicator that shows the relationship between two moving averages of a security’s price. The MACD is calculated by subtracting the 26-period exponential moving average (EMA) from the 12-period EMA.
> 
> Formula:
> $$MACD = EMA_{12Days} - EMA_{26Days}$$

> ## **Signal Line** <br>
> Moving average convergence divergence (MACD) is a trend-following momentum indicator that shows the relationship between two moving averages of a security’s price. The MACD is calculated by subtracting the 26-period exponential moving average (EMA) from the 12-period EMA.
> 
> Formula:
> $$MACD = EMA_{12Days} - EMA_{26Days}$$

> ## **Histogram** <br>
> MACD is often displayed with a histogram (see the chart below) which graphs the distance between the MACD and its signal line. <br>
> Traders use the MACD’s histogram to identify when bullish or bearish momentum is high.
> 
> Formula:
> $$Value = MACD - SignalLine$$

## One of the main problems with divergence is that it can often signal a possible reversal but then no actual reversal actually happens—it produces a false positive. The other problem is that divergence doesn't forecast all reversals. In other words, it predicts too many reversals that don't occur and not enough real price reversals.
## "False positive" divergence often occurs when the price of an asset moves sideways, such as in a range or triangle pattern following a trend.