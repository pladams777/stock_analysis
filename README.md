# An Improvement on the Analysis of Green Stocks
Refactoring code used to analyze stock performance over a given year.
## Project Overview
With this project we took code that was written in prior lessons and refactored it to improve efficiency. The purpose of both the original and refactored code is to analyze stocks, specifically green energy stocks. The dataset used contains daily trading information for 12 green energy stocks in two given years. The intention by refactoring the existing code is to create a subroutine that will efficiently analyze a much larger number of stocks, potentially the entire stock market over the last few years. 

## Results
The original code was written to analyze 12 specific stocks. There are 252 trading days per year which multiplied by 12 stocks left us with over 3000 rows of data. The original code cycled through the entire dataset over and over for each different stock.

In an attempt to improve efficiency, we refactored the code to only have to cycle through the data one time by utilizing multiple arrays. The hope is that with improved speed and efficiency, the refactored code will be able to analyze a much larger dataset in a reasonable amount of time.

### The refactored code reduced the run-time of the original code by more than 80%.

### Times for given year using *Original Code*:

![green_stocks_2017](https://user-images.githubusercontent.com/107540080/177075794-ea8702f1-812b-4b3e-bb90-885319624301.png),![green_stocks_2018](https://user-images.githubusercontent.com/107540080/177075800-28284564-ca11-42b0-8860-b0bfe9d49163.png)

### Times for given year using *Refactored Code*:

![VBA_Challenge_2017](https://user-images.githubusercontent.com/107540080/177075533-cfa9ecdb-baef-4f6d-becb-8fed3cb44ef5.png),![VBA_Challenge_2018](https://user-images.githubusercontent.com/107540080/177075573-a73dddae-efad-4281-af90-112cd11204b7.png)

## Summary
There can be both **Pros** and **Cons** to refactoring code. One advantage can be efficiency as shown in our example. Refactoring can often lead to faster running code that takes up less machine resources. Disadvantages can be that doing so may exceed a given budget or time limit to create a certain project.

When refactoring the original Stock analysis code, the biggest disadvantage was time: the time it took to rebuild and debug the refactored code. But this was definitely outweighed by the advantage of a more efficient code.
