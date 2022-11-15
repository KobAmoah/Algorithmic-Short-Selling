# Algorithmic-Short-Selling
          Our life is frittered in detail ... simplify, simplify.
                                                                    - Henry David Thoreau

  This work aims to strip a trading system to its core - trading rules. In particular, 
the focus is on simple trading rules since it much easier to explain the 
profitability and behavior of such rules. 

  While a trend analysis forms the basis of the project's implementation, the
wider aim of the project is to answer the following fundamental questions
-    What makes a good trading rule? 
-    When does the rule work and why does it work?      
-    How successful should you expect to be by trading that rule?
-    How would this rule fare when you have a limit on how much you can lose?

         What exactly is the strategy?
# Moving Average Price with Volatility Bands on the Exxon Mobil Stock('XOM')
 How it does the strategy work?

 - Enter when today's price exceeds the   MA price + s * atr 
 - Exit when today's price goes below the MA price - s * stdev
 - Else maintain your prior position

 atr = average true range, and s = scaling factor
 
          How is the code organized?
 # Code Organization & Functions 

- Section 1.  Library Imports

- Section 2.  Data Imports and Conversion to Relative Price Series 
 
- Section 3.  Moving Average Strategy 

- Section 4.  Gain Expectancies   

- Section 5.  Risk Management & Performance Metrics  
                     
- Section 6.  Drawdown  

- Section 7:  Summary (Strategy Stats) 


# How does the Strategy Perform?


<img width="589" alt="Screenshot 2022-11-14 at 6 37 16 PM" src="https://user-images.githubusercontent.com/108365002/201797652-f58697bf-5c92-4346-a7b8-07a6bdc55c02.png">

     
