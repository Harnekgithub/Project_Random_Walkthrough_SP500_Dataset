# Project Random Walkthrough SP500 Dataset
Measuring the ability of random individual stock selection vs professional managed portfolio

In 1973, Princeton University economics professor Burton Malkiel made a bold claim in what went on to become his best-selling book “A Random Walk down Wall Street” that “A blindfolded monkey throwing darts at a newspaper’s financial pages could select a portfolio that would do just as well as one carefully selected by experts”. In the almost 50 years since professor Malkiel first published his book, now in its 12th edition, an unlimited amount of stock return data has given us infinite opportunities to test out his theory, and what we’ve learned, unequivocally, and what we will demonstrate to you today, is that the professor was wrong.

To get an idea of how professional money managers performed, we sought out highly-rated Large-Cap blend mutual funds, and charted their performance over a 20-year period, from January 1, 2020, to December 31, 2019. We analyzed the mutual fund performance by assuming an investor bought exactly $10,000 worth of mutual fund shares on January 1, 2020, and measuring what the balance would be on December 31, 2019 if that investor never any more added money to, or withdrew from their mutual fund over the entire measurement period.

List of stocks that make SP500 October 2021 was pulled from Wikipedia and data was cleaned and scrubbed to have consistent data for all stocks that we can pick randomly.
  - All the stocks that were added between 1901-01-01 and 2000-01-01 were selected to have data from 2000-01-01 through 2019-12-31
  -	Stocks that had no date when they were added to SP500 were dropped.
  -	This gave us a list of 160 stocks to choose from
  
We used df.sample() function to get random stocks from the list.

Once the list was compiled yfinance download function was used to get the monthly data points from Yahoo.com Findings were inline with our quest to see if random selection can be as good as professionally managed funds? We were 'Totally Wrong' Randomly picked portfolios over performed compared to the professionally managed most of the time.

10 Portofilos of 5, 10 and 15 randomly picked stocks performance were compared to 

## FLCSX,  HAIAX,  DFUSX,  PRBLX,  DGAGX,  TISCX,  VDIGX,  DFELX,  MRGAX,  BRLIX

Charts below show the outcome from one such iteration.

![Managed Funds](./images/Historical Chart for Managed Funds.png)  

![5 Stock Random Portfolios](./images/Comparison of Average of all portfolios with 5 stocks in them vs managed funds.png)

![10 Stock Random Portfolios](./images/Comparison of Average of all portfolios with 10 stocks in them vs managed funds.png)

![15 Stock Random Portfolios](./images/Comparison of Average of all portfolios with 15 stocks in them vs managed funds.png)

