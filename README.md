java c
25762
Derivatives and Risk Management
Spring 2024
CASE STUDY
Due on Tuesday 29 October 2024 at 5:00pm
Learning Objectives
By completing this case you will learn to:
-      Learn about trading strategies with options
-      Learn to compute option implied volatilities
-      Learn  about  using  implied  volatilities  to  provide  pricing  and  option  structure information for OTC FX derivatives
-      Understand   the   interaction   between   option   prices,   strike   prices,   time   to expiration and volatility
-      Communicate complex analysis to anon-technical audience.
Learning Activities
By completing this case you will:
-      Explain trading strategies such as risk reversals and strangles
-      Use implied volatility data and option deltas to back out option prices and strike prices
-      Use  implied volatility data from option strategies to back out option prices and strike prices
-      Use interpolation methods to estimate implied volatilities for a related option
-      Plot and interpret a volatility surface
-      Write an executive report for a non-technical audience
TaskYou are an associate at a Sydney commercial bank. One of the bank’s commercial clients has been looking into FX options and came across reporting conventions for OTC FX options and options strategies that they did not understand.The client has asked you to write a brief report to explain how options strategies such as risk reversals and strangles work, how implied volatilities can be used to summarize information about option prices and the role of the option deltas in options pricing. You need to write a clear description of how it is possible to represent options prices and strike prices through information about implied volatilities and option deltas. Your report is targeted to a relatively non-technical reader – someone who has a very rudimentary understanding of the  Black- Scholes-Merton formula and option payoutson expiration.You find some examples of implied volatilities for European options and for European option positions  in the  British  Pound  (GBP)  in term  of  US  dollars  (USD)  over a two-week  period (trading days from 4 April through 15 April). These implied volatilities are computed from option prices using the Black-Scholes-Merton model for currency options.
Table 1 gives the spot price of one British Pound in terms of US Dollars as well as the implied volatilities of USD-denominated options written on the GBP during this period:
Table 1: Implied Volatilities of 50-delta calls on GBP
Date
Spot Rate
Implied Volatilities of 50-delta calls


1 Week
1 Month
3 Month
6 Month
1 Year
4 April
USD1.3216
7.23%
7.455%
7.905%
8.07%
8.27%
5 April
USD 1.3174
7.645%
7.915%
7.935%
8.105%
8.285%
6 April
USD 1.3169
7.785%
7.935%
8.005%
8.19%
8.335%
7 April
USD 1.3175
7.61%
7.655%
7.94%
8.15%
8.31%
8 April
USD 1.3125
7.205%
7.51%
7.835%
8.035%
8.25%
11 April
USD 1.3130
6.86%
7.74%
7.82%
8.045%
8.25%
12 April
USD 1.3101
6.24%
7.49%
7.66%
7.93%
8.165%
13 April
USD 1.3217
6.32%
7.365%
7.62%
7.85%
8.11%
14 April
USD 1.3171
6.17%
7.18%
7.35%
7.675%
7.985%
15 April
USD 1.3165
6.4%
7.195%
7.35%
7.69%
7.985%The volatilities quoted above apply to so-called “50-delta calls," which means to say they are the volatilities of USD-denominated European calls on the GBP whose strike prices are chosen so that their deltas are 0.5.Table 2 gives market implied volatilities for two different option strategies. The first strategy is known as a “25-delta reversal" and is a combination of a long out-the-money European call with a delta of 0.25 and a short out-the-money European put with a delta of -0.25. The second strategy is a “25-delta strangle" which is a combination of along out-the-money European call with a delta of 0.25 and a long out-the-money European put with a delta of -0.25. This table provides  market  implied vol代 写25762 Derivatives and Risk Management Spring 2024Java
代做程序编程语言atilities for  USD-denominated  25-delta  reversals  and  25-delta strangles on the GBP with different maturities, over the period 4 to 15 April:
Table 2: Implied Volatilities of 25-Delta Risk Reversals and 25-Delta Strangles
Date
25-Delta Risk Reversals
25-Delta Strangles

1 Month
3 Months
1 Year
1 Month
3 Months
1 Year
4 April
-0.98%
-1.195%
-1.505%
0.37%
0.48%
0.63%
5 April
-0.92%
-1.155%
-1.515%
0.36%
0.48%
0.63%
6 April
-0.90%
-1.105%
-1.535%
0.37%
0.48%
0.63%
7 April
-0.88%
-1.135%
-1.485%
0.37%
0.47%
0.63%
8 April
-0.91%
-1.175%
-1.495%
0.37%
0.46%
0.63%
11 April
-0.95%
-1.185%
-1.505%
0.35%
0.46%
0.63%
12 April
-0.94%
-1.18%
-1.525%
0.35%
0.48%
0.63%
13 April
-0.97%
-1.185%
-1.535%
0.36%
0.48%
0.63%
14 April
-0.94%
-1.195%
-1.50%
0.36%
0.47%
0.63%
15 April
-0.91%
-1.195%
-1.515%
0.35%
0.47%
0.63%
The following market conventions apply to the implied volatilities quoted above:
•    the listed volatility of a 25-delta reversal is the volatility of the underlying call minus the volatility of the underlying put;
•    the  listed  volatility  of  a  25-delta  strangle  is  the  average  of  the  volatilities  of  the underlying call and put minus the volatility of the corresponding 50-delta call.
Further, assume that the continuously compounded risk-free interest rates in the UK and the US are 3.50% and 2.30%, respectively for all maturities.
The following analysis is required to be performed in the spreadsheet and will inform. the content of your report:
Part A
•    Convert the  implied volatility  data from Table 1 into a table with the option strike price associated with each implied volatility value. Be sure to explain to your client what you have done and why, in addition to presenting how the strike price has been computed in the spreadsheet.
•    Compute the option price for each of these strike prices.
•    Comment on any trends  in the option price over these 10 trading days and provide potential explanations of these trends (for different option maturities).
Part B
•    Use Table  2 to  compute the strike  price for each call and put used in the 25-delta reversals and 25-delta strangles for each date. Be sure to explain to your client what you have done and why, in addition to presenting how these strike prices have been computed in the spreadsheet.
•    Explain to your costumer the role, potential gain/loss and risk profile of reversals and strangles. Why are you using these strategies to construct implied volatility surfaces? In  the  spreadsheet  demonstrate  the  profit/loss   profile  of  the  3-month  25-delta reversal and a 25-delta strangle traded on 7 April.
•    Explain  the   meaning  of  options  delta   in  relation  to   moneyness  and   its  role  in computing strikes prices and option prices.
Part C
•    Illustrate how Part A and Part B can be used to value other options with the following example. Suppose on 7 April you bought a one-month European call on 150,000 GBP with a strike of USD 1.32 per GBP and on 14 April you sold a three-month European put on 100,000 GBP with a strike of USD 1.35 per GBP. In the spreadsheet show how, by using linear interpolation across strikes, you can estimate the implied volatilities for these two options and hence determine their corresponding price.
•    Explain to your  client  how  information from these tables  can be used to estimate implied volatilities of other options and hence value any other option.
Part D
•    In the spreadsheet, plot the volatility surface (implied volatility as a function of the strike price) for these two options of part C with one-month, 3-month and 1-year time to maturity on 7 April and 14 April.
•    Present and explain to your client the volatility surface and its importance. Are there any noticeable patterns or surprises on these surfaces, on these two days?



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
