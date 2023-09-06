### **Tesla's stock data analysis from 6/29/10 to 3/24/22 by Lucio Awa**

#### Source of data: [Kaggle](https://www.kaggle.com/datasets/varpit94/tesla-stock-data-updated-till-28jun2021)

#### Programs used:

- SQL
- Python with Pandas
- Matplotlib + Seaborn

#### I. 	INTRODUCTION

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

#### II. 	QUERIES and analysis in 'Tesla_Stock_Prices.ipynb' 

These queries are essential for various aspects of financial analysis, including risk assessment, trend identification, and decision-making in trading and investing. They provide valuable insights into market behavior and help stakeholders make informed choices. 

##### Format of analysis for each query:¶

- SQL query
- Python with Pandas dataframe
- Matplotlib + Seaborn Visualization
- Insights gained about Tesla's stock

**1. Basic Summary Statistics**

This query provides essential statistical information about a financial dataset. It typically includes measures like mean (average), median (middle value), standard deviation (variability), minimum (lowest value), and maximum (highest value) for variables such as closing prices or trading volumes.

Basic summary statistics give a quick overview of the dataset's central tendency, spread, and potential outliers. They are fundamental for understanding the distribution and behavior of financial data, helping investors and analysts make informed decisions.

**2. Yearly Average Closing Prices**

Yearly average closing prices provide a broader perspective on a stock's performance. They help identify long-term trends and can be used for comparing performance across different years.
   
**3. Highest Volume in a day with corresponding Maximum Volume for each year**

This query finds the highest trading volume for a single day in each year and provides the corresponding maximum volume value. Identifying days with exceptionally high trading volumes can signal significant market events or changes in sentiment. This information is crucial for understanding market dynamics and potential price movements.
   
**4. 10-day moving average of closing prices around Tesla's Highest Volume day**

This query calculates the moving average of closing prices over a 10-day window centered around a specific date, such as 2020-02-04 wich is Tesla's highest volume day. Moving averages help smooth out short-term fluctuations, making it easier to spot trends and potential reversals. They are commonly used by traders and investors for technical analysis.
   
**5. Days with Significant Price Change around Tesla's Highest Volume day**

This query identifies days when a stock's price changed significantly, often defined as a certain percentage change. Detecting days with substantial price changes can highlight events or news that had a significant impact on the stock. This information is valuable for understanding market volatility.
   
**6. Yearly low and high range of Tesla's stock prices**

This query calculates the annual low and high prices for a stock. Yearly low and high ranges provide insight into a stock's price volatility within a year. This data can help investors set realistic expectations and risk management strategies.
   
**7. Volume and Close Price Correlation**

This query computes the correlation between trading volume and closing prices. Correlation analysis helps assess the relationship between trading activity (volume) and price movements. Positive correlations suggest that higher trading volumes coincide with price increases, while negative correlations imply the opposite. This information aids in understanding market dynamics and investor sentiment.

#### III	OVERALL INSIGHTS GAINED FROM QUERIES

A detailed analysis of each query ia located in the 'Tesla_Stock_Prices.ipynb'. These are the overall insights gained from each query:

**1. Basic Summary Statistics**

From the basic summary statistics, we've learned that Tesla's stock has shown substantial growth and significant volatility. The price range from $22.79 to $1229.91 indicates long-term growth potential, attracting both short-term traders and long-term investors. However, this wide price range also signifies the stock's high volatility, influenced by market sentiment, external factors, and investor behavior. Traders and investors have had opportunities for significant gains or losses, and understanding this volatility is crucial for risk management. The average closing price of $138.76 provides an overview of the stock's performance, while the standard deviation of $250.12 indicates substantial price fluctuations around the mean, reflecting its volatile nature. To gain deeper insights, it's essential to consider historical events and trends that may have contributed to these price movements.

**2. Yearly Average Closing Prices**

The analysis of yearly average closing prices reveals distinct phases in Tesla's stock performance: early growth, rapid expansion, stabilization, explosive growth, and continued strength, influenced by market sentiment, investor behavior, and external events, highlighting the stock's long-term growth potential, volatility, and the need for informed investment strategies.

**3. Highest Volume in a day with corresponding Maximum Volume for each year**

The patterns in maximum trading volume for Tesla's stock on specific dates and in particular years are shaped by global financial events, Elon Musk's companies' developments, and broader market dynamics, indicating the influence of economic conditions, investor sentiment, and visionary leadership on trading activity.

**4. 10-day moving average of closing prices around Tesla's Highest Volume day**

The 10-day moving average analysis around Tesla's Highest Volume day in 2020-02-04 indicates an upward trend in the stock's price leading up to that date, with a significant spike in both the closing price and the moving average on that specific day, likely due to a significant event or news, accompanied by notable volatility and trading patterns during this period.

**5. Days with Significant Price Change around Tesla's Highest Volume day**

During the specified time frame around Tesla's Highest Volume day, there were periods of both upward and downward trends in the stock's prices, with the most significant price changes occurring around February 3 and February 4, accompanied by notable volatility and market sentiment shifts.

**6. Yearly low and high range of Tesla's stock prices**

The yearly low and high ranges of Tesla's stock prices demonstrate the company's evolution from early volatility and innovation to becoming a global leader in the electric vehicle industry, with key milestones, market recognition, and periods of significant growth shaping its market perception and valuation.

**7. Volume and Close Price Correlation**

The correlation coefficient of 0.0906 indicates a very weak positive linear relationship between Tesla's closing prices and trading volumes, suggesting that changes in trading volume have limited predictive power for changes in stock prices, and other factors like news and market sentiment play a more significant role in driving price movements.

#### IV	CONCLUSION

The following three terms and questions provide a foundation for evaluating the suitability of a stock as an investment. They consider the rationale behind the investment, the associated risks and rewards, and the strategic fit within the broader context of the company's or investor's financial objectives and portfolio strategy:

**1. Investment Thesis**: What is the fundamental reason for considering Tesla's stock as an investment?

Tesla's stock has demonstrated significant growth and volatility over the years, with periods of rapid expansion. The fundamental reason for considering Tesla's stock as an investment lies in its history of significant growth and market leadership in electric vehicles and sustainable energy.

**2. Key Risks and Rewards**: What are the primary risks associated with investing in Tesla, and what are the potential rewards?

Tesla's stock exhibits a wide range of prices, indicating substantial volatility and the potential for both gains and losses, which presents opportunities but also requires careful risk management. Risks include market sentiment shifts, external factors, and the potential for rapid price swings. The potential rewards include the opportunity to benefit from Tesla's innovative leadership and its position in the growing electric vehicle and sustainable energy sectors.

**3. Portfolio and Strategy Alignment**: How does investing in Tesla align with an investor's existing portfolio or corporate strategy, which is to maximize gains in short and long term investments? 

Tesla's stock has gone through different phases, from early volatility to becoming a global leader in the electric vehicle industry. These fluctuations can be influenced by a wide range of factors, including market sentiment, news events, and even social media posts by Tesla's CEO, Elon Musk.

Investing in Tesla for short-term gains can be unpredictable due to the stock's high volatility. Short-term investors should be cautious and have a well-defined trading strategy that includes clear entry and exit points, stop-loss orders to limit potential losses, and staying informed about market news. While the potential for gains exists, it's essential to manage risk carefully when pursuing short-term investment objectives in Tesla's stock.

Long-term investors in Tesla can benefit from its growth potential in the electric vehicle and sustainable energy markets. While there may still be volatility over the long term, Tesla's innovations and market position make it an attractive option for investors with a patient investment horizon. Aligning Tesla with a long-term portfolio strategy can capitalize on the company's potential to disrupt industries and drive sustained growth over time, provided investors are prepared for periodic market fluctuations.

In conclusion, for potential investors considering Tesla's stock involves recognizing its history of significant growth and leadership in electric vehicles and sustainable energy, with opportunities for substantial rewards but also the need for careful risk management due to its notable volatility, making it a more favorable option for long-term investors aligned with its innovative potential.


