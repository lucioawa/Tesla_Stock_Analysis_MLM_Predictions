# Tesla_Stock_Analysis From 6/29/10 to 3/24/22

# Source: https://www.kaggle.com/datasets/varpit94/tesla-stock-data-updated-till-28jun2021

# by Lucio Awa

# Programs used for queries, data frames, and visualizations:
# SQL
# Python with Pandas + Matplotlib + Seaborn

I. 	INTRODUCTION

The following terms refer to various data points that describe the trading activity and price movement of Tesla's stock on a particular trading day:

1. Date: This is the specific trading date on which the stock market was open and trading occurred.

2. Open: Initial price at which the stock started trading.

3. High: The highest price that buyers were willing to pay for the stock on that day.

4. Low: The lowest price that sellers were willing to accept for the stock on that day.

5. Close: The closing price is the last trade executed before the trading session ended.

6. Adjustment_Close: The adjusted closing price takes into account any corporate actions or other events that could affect the value of the stock. 

    The adjusted price accounts for the impact of these events on historical stock prices, allowing investors and analysts to compare performance over time on a more consistent basis. 
    Here is more detail about each event:

      A. Stock Split: A stock split is a corporate action in which a company divides its existing shares into multiple shares. For example, in a 2-for-1 stock split, each existing
         share is split into two new shares. The total value of the shares remains the same, but the number of shares outstanding increases. Stock splits are often done to make the
         stock more accessible to a larger number of investors, and they can also increase liquidity. 

         When a stock split occurs, the historical stock price is adjusted proportionally to reflect the split. For instance, if a stock was trading at $100 per share before a
         2-for-1 stock split, after the split, the price would be adjusted to $50 per share. The adjusted close price takes into account these splits so that the historical price
         charts remain consistent and comparable.

      B. Dividend Distribution: A dividend is a payment made by a company to its shareholders from its profits. It is a way for companies to share their earnings with investors.
         Dividends can be paid in the form of cash or additional shares of stock, known as a stock dividend. When a company issues a dividend, the stock price tends to decrease by
         the amount of the dividend payment because the company's value is being distributed to shareholders.

         For example, if a company's stock is trading at $100 per share and it pays a $2 dividend, the stock price might drop to $98 to account for the distribution of the dividend.
         The adjusted close price also takes into consideration the impact of dividends, ensuring that historical price charts accurately reflect the overall return an investor would
         have received.

      C. Bonus Issues or Stock Dividends: Similar to regular dividends, bonus issues involve the distribution of additional shares to existing shareholders instead of cash. This can
         impact the adjusted price of the stock.

      D. Rights Offerings: When a company offers its existing shareholders the right to purchase additional shares at a discounted price, it can lead to changes in the adjusted price.

      E. Mergers and Acquisitions: If a company is acquired or merges with another company, the adjusted price of the stock may be affected based on the terms of the deal, such as
         exchange ratios or cash payments.

      F. Spin-offs: When a company separates a portion of its business into a new independent company, the adjusted price of the original company's stock might change.

      G. Stock Buybacks: Companies repurchasing their own shares can impact the adjusted price, as it affects the total number of outstanding shares.

      H. Initial Public Offerings (IPOs): When a company goes public, its stock is introduced to the market. The adjusted price can be influenced by factors such as demand, pricing,
         and the overall performance of the IPO.

      I. Earnings Announcements: Positive or negative earnings reports can lead to significant changes in stock prices, which will affect the adjusted price as well.

      J. Changes in Management or Key Personnel: Announcements of changes in top leadership or key personnel can impact investor sentiment and, consequently, the adjusted price.

      K. Regulatory Changes: Changes in regulations or legal developments that affect the company's operations can influence the stock's adjusted price.

      L. Macroeconomic Factors: Economic indicators, interest rates, inflation, and other macroeconomic factors can influence investor behavior and impact the adjusted price.

      M. Industry or Sector News: Developments specific to the industry or sector in which the company operates can affect its stock price and adjusted price.

      N. Market Sentiment: Overall market sentiment, investor perception, and market trends can impact stock prices and adjusted prices.

      O. Geopolitical Events: Events like political instability, conflicts, or international relations can impact stock markets and, consequently, the adjusted price of stocks.

      P. Natural Disasters: Major natural disasters or catastrophes that affect a company's operations can influence its stock price and adjusted price.

7. Volume: Volume refers to the total number of shares of a company's stock that were traded on that trading day. It gives an indication of the level of activity and interest in
   the stock on that particular day. Higher volume often suggests increased market interest and liquidity.

   Traders and investors use this information to analyze trends, make investment decisions, and assess the overall market sentiment towards a particular stock.

II. 	QUERIES: 

Queries presented in SQL detailing what each line does, then using Python with Pandas in Jupyter Notebooks + Matplotlib + Seaborn for visualizations, ending with conclusions and insights
gained based on each query. 

1. Basic Summary Statistics
2. Yearly Average Closing Prices
3. Highest Volume in a day with corresponding Maximum Volume for each year
4. 10-day moving average of the closing prices for Tesla's stock around the date 2020-02-04 with 10 rows as a result
5. Days with Significant Price Change
6. Yearly low and high range of Tesla's stock prices
7. Volume and Close Price Correlation


