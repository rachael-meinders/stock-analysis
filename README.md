# stock-analysis
Bootcamp - Analysis of Stock Volume and Return using VBA

## Overview
This analysis seeks to explore and analyze twelve different green energy stock volumes and returns for the years 2017 and 2018. This analysis utilized VBA coding in Excel. Methodology for this analysis included nested for loops, running through our twelve stocks and through each day's stock performance to extract key performance points. Performance is then evaluated through the daily volume of each stock as well as the returns it generated over the course of the year. 

![Performance_output](https://user-images.githubusercontent.com/90879979/136491524-ae2b4865-36be-4d85-8b47-270cdd384f8f.png)

To optimize the performance of the analysis, my refactored code introduces tickerIndex as way of internally generating the entire portfolio's performance before outputting each stock's results. This increased efficiency, resulting in decreased run-times and ease in expanding the scope of the dataset in the future.

![tickerIndex](https://user-images.githubusercontent.com/90879979/136491596-24315350-ef5c-45db-b0df-550eebc511a0.png)

## Results (screenshots)
### 2017 vs 2018 
Overall, 2017 was a successful year for our selected stocks, resulting in positive returns for eleven out of our twelve selections. These successful stocks faced both moderate returns of 5-30% and almost explosive returns of more than 100%. The one declining stock had a somewhat reasonable decline of only 7.2% with a total volume of 139 million.   

On a whole, 2018 was a very unsuccessful year for our selected stocks with only two out of twelve with a positive return. While it is certainly true that all markets are volatile, the swing between overall success to overwhelming failure of these stocks seems to extend past market volatility. Government policy changes and pushes may have also played a part in these negative returns and is definitely an area worth further exploration. Nonetheless, such negative returns may sugguest that the selected stocks represent generally underwhelming companies or companies that are currently facing significant obstacles, in which case I strongly suggest we expand the data set to include a diversified set of stocks. This diversity represents a better portion of the whole and allows us to better observe overall market volatility in comparison to the true value of a comapany's continuing performance.

In looking at these two years of stocks results, ENPH and RUN stand out as they are the only stocks to have positive returns both years. However, ENPH edges out its competitors as it has had impressively large returns - 130% and 82%. These two large returns indicate a history of sucess as well as a potential for further positive returns. While extending our analysis to include a longer history of these stocks would increase our knowledge of and confidence in these assumptions, I recommend that my client strongly consider investing first in ENPH and then in RUN.

![Best_performers](https://user-images.githubusercontent.com/90879979/136491620-178ec196-ce7f-4365-9729-8338448ceba1.png)

### Analysis Run-Time 
In my original code, running strictly the analysis (without formatting) ran in roughly 1.25 seconds. While this certainly isn't horrible, it can still use improvement, especially since I was able to watch the code print the values line by line. I don't believe this is necessarily a negative quality, I want to give my client a high-quality, efficient code. In an effort to produce work of this caliber, adding in the tickerIndex to the refactored code cut the run-time to nearly 1/9th of the original at just over .17 seconds.

![Original_timer](https://user-images.githubusercontent.com/90879979/136491642-592ed706-f8a3-4b29-94c9-601e847590c2.png)
![Refactored_timer](https://user-images.githubusercontent.com/90879979/136491663-354bc6fc-4904-4c99-b533-a18b58fed15b.png)

## Summary
In the previous practice code, increasing the number of tickers that are analyzed would only slow down the analysis run time. If the client is considering a much broader scope of analysis, the original code likely would become cumbersome to run due to the slow run-time. Specifically, printing the ticker, totalVolume, and Return line by line, ticker by ticker would become frustrating to watch. The refactored code, however, would generate the entire analysis internally first, then output it all at once. Overall, this is a more pleasant client experience as I think we would all be a bit more patient with a computer taking a bit more time computing rather than printing. 

