![fce324cd220e0ec9435bebbfceb50cc2](https://user-images.githubusercontent.com/108365002/203485165-311a3631-807e-4906-b27b-2566779dbb43.jpeg)

# Algorithmic-Short-Selling
          Our life is frittered away by detail.... Simplicity, 
          simplicity, simplicity! I say, let our affairs be 
          as two or three, and not a hundred or a thousand
          ...Simplify, simplify!
                                                                    - Henry David Thoreau

  This work aims to strip a trading system to its core - trading rules. More so, 
the focus is on simple trading rules since it much easier to explain the 
profitability and behavior of such rules. 

  While a trend analysis forms the basis of the project's implementation, the
wider aim of the project is to answer the following fundamental questions
-    What makes a good trading rule? 
-    When does the rule work and why does it work?      
-    How successful should you expect to be by trading that rule?
-    How would this rule fare when you have a limit on how much you can lose?

         So, what exactly is the strategy?
# Moving Average(MA) Price with Volatility Bands on the Exxon Mobil Stock('XOM')

 - You enter when today's price exceeds the   MA price + s * atr 
 - You exit when today's price goes below the MA price - s * stdev
 - Else you maintain your prior position

 atr = average true range, and s = scaling factor
 
 # Altering the Definition of the Moving Average Price
 
 Rather than using the raw prices, prices are rebased/ expressed relative to the benchmark 
 for the strategy to be viable. Rebasing is defined in the following way, 
 (current stock price/current benchmark value) * first value of benchmark in its price series.
 
 # What does this exactly mean? 
 
 Suppose the data starts on January 4, 2008 and today's date 
 is December 13, 2011, the relative price series is given by 
 (stock price on 12/13/2011 / benchmark value on 12/13/2011) * benchmark value on 01/04/2011.
 
 # Implemented form of strategy
           RMA = Relative Moving Average
 - You enter when today's price exceeds the   RMA price + s * atr 
 - You exit when today's price goes below the RMA price - s * stdev
 - Else you maintain your prior position
 
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

Disclosure: This work was inspired by initial work done by Laurent Bernut
     
