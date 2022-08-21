# Formulaic Alpha-22 Quantitative Trading Strategy
> - Credit to Zura Kakushadze, Ph.D. at Quantigic® Solutions LLC and University of Tbilisi, Business School & School of Physics
> - Article Source: https://arxiv.org/ftp/arxiv/papers/1601/1601.00991.pdf
> - Abstract: <br>
> Their average holding period approximately ranges 0.6-6.4 days. The average pair-wise correlation of these alphas is low, 15.9%. The returns are strongly correlated with volatility, but have no significant dependence on turnover, directly confirming an earlier result based on a more indirect empirical analysis. We further find empirically that turnover has poor explanatory power for alpha correlations. 
> The alphas described in the article is restricted to some extent as they are proprietary to WorldQuant LLC.

<br>

## Concetps
> #### Delay-n Alpha
> - Generally, **delay-n** means that some data in the alpha is used for trading **after n day(s)**.
> - e.g., delay-0 alpha uses today's data for today's trades.

> #### Mean-reversion Alpha (delay-0)
> - A mean-reversion alpha has a sign opposite to the return on which it is based, and the basic idea is that a stock would have a elastic recover from its gain/loss yesterday.
> - Simple mean-reversion alpha: <br> $$ln(open_{today}/close_{yesterday})$$	
> - The close is adjusted for splits and dividends.

<br>

> #### Momentum Alpha (delay-1)
> - The basic idea is that if a stock went up/down yesterday, the trend will continue today.
> - Simple mean-reversion alpha: <br> $$ln(close_{yesterday}/open_{yesterday})$$

<br>

# to be continued...