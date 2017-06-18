# What's in the numbers: A look at the Lusaka Securities Exchange
Aaron Simumba  
June 18, 2017  



In the next coming few weeks, I plan to do a series of posts specifically targeted at the Lusaka Securities Exchange (LuSE). Essentially, this idea came to mind after reading through this [Bloomberg Markets](https://www.bloomberg.com/news/articles/2017-01-10/history-shows-world-s-best-stock-gains-arise-in-emerging-markets) article, which highlights historical equity market returns . One aspect that stands out from this article is that over the past 2 decades, emerging markets equities provided greater returns; both on a risk adjusted basis and in dollar terms.
And of focus here, the LuSE, ranks in the top 10 on both account of returns after converting to US dollars and on a risk adjusted basis. The table below shows the local bourse appearing twice in the top ten, twice  on number 2 in the year 2007 and 2011 only being edge out of the first spot by Mongolia on both occasions.
As this data from Bloomberg Markets  shows, emerging and frontier markets accounted for 9 spots out of a rank order of 10 in dollar terms and 7 spots on a risk adjusted basis.





The following excerpt from Bloomberg stands out:

     “The top 10 stock indexes that gave global investors the greatest returns in 2016 were all emerging or frontier markets, according to data compiled by Bloomberg. That’s not a fluke: over the past 20 years, nine out of 10 best-performing equity gauges have been in developing nations, the figures show”.

Investment theory contends that risk taken in an investment must commensurate the return sought. Though equities as a class of investible assets are by their very nature riskier assets relative to other assets like Treasury Bill or Bonds; this in essence frightens most investors to invest in them. More so from the view of the emerging markets, which expose investors to higher levels of volatility relative to more mature and developed markets. In my next post I will look at what was historically being  demanded by investors for taking up the extra risk posed by emerging markets.

The table below shows the top 10 market returns on a risk adjusted basis. No doubt emerging markets still dominated the list.




What’s impressive from this table is that from the period 1997-2016, Zambia appears 5 times, occupying the first position once in the year 2013. The country appeared 4 within the top 5 spots in terms of risk adjusted equity returns in the world .In local currency terms this reflected an over 40% return as can be seen from figure 4.0 below. Going forward, investors can remain optimistic on the prospects of the emerging markets delivering stellar returns ahead of the developed markets pack. So far, the MSCI Emerging Markets Index has gained 2.7 percent in comparison with 1.5 percent from developed stock markets.

## In Focus

The following charts give a snapshot of the performance of the Lusaka Securities  Exchange All Share index (LASI). For the monthly index data, the period covered is from January 2005 to December 2014. As for the yearly data, it goes all the way back to January 1997- December 2014. Furthermore, I present the data on both time intervals, inclusive and exclusive of the Zambia Consolidated Copper Mines Investment Holdings (ZCCM-IH). This is simply to highlight the effect that the company has on the market index as a whole and on the bigger side, the nation's economy.

NB: The returns are computed in the local currency (Kwacha).


```r
plot(LASI_monthly$Return, xlab=" Period", ylab="Return",main="The LuSE LASI Monthly Returns For the Period 2005-2014
     (excl. ZCCM-IH)",cex.main =1, font.main=2)
```

![](2017-07-18-luse-analysis_files/figure-html/unnamed-chunk-4-1.png)<!-- -->


Most noticeable from the above chart is the greater volatility experienced at the on set of the Global financial crisis. At the height of this crisis we see the index slumping close to -40.0%, conversely, also it hit a record high of more than 60.0% return. The index overall performance is an up-down swing with periods of decent returns and other periods of downward performance.

## Monthly Returns Inclusive of ZCCM-IH


The following chart shows the LASI index inclusive of  ZCCM-IH. Since the LASI is a value weighted index, stocks having greater market value tend to have a much more pronounced effect on the movement in the index. For instance, factoring ZCCM-IH’s market capitalization into the LASI index has a telling effect on the overall picture of the index. The chart below shows volatility in certain months relatively lower compared to the chart above which excludes ZCCM-IH. My follow-up posts will closely evaluate this effect and try to elicit some information that explains why this is the case.


```r
plot(LASI_monthly_zccm$Return,xlab=" Period", ylab="Return", main="The LuSE LASI Monthly Returns For the Period 2005-2014 
     (incl. ZCCM-IH)",cex.main =1, font.main=2)
```

![](2017-07-18-luse-analysis_files/figure-html/unnamed-chunk-5-1.png)<!-- -->

The last two charts detail the index on a yearly basis. Though unlike the picture painted from the monthly data, yearly data that goes farther down the years, seem to be carrying a different message on the effect of the company ZCCM-IH. When introduced into the computations, the volatility is more than that observed without its inclusion.

```r
plot(LASI_yearly$Return,xlab=" Period", ylab="Return", main="The LuSE LASI yearly Returns For the Period 1997-2014 
     (excl. ZCCM-IH)",cex.main =1, font.main=2)
```

![](2017-07-18-luse-analysis_files/figure-html/unnamed-chunk-6-1.png)<!-- -->

__Inclusive of ZCCM-IH yearly LASI Index returns__

```r
plot(LASI_yearly_zccm$Return, xlab=" Period", ylab="Return", main="The LuSE LASI yearly Returns For the Period 1997-2014 
     (incl. ZCCM-IH)",cex.main =1, font.main=2)
```

![](2017-07-18-luse-analysis_files/figure-html/unnamed-chunk-7-1.png)<!-- -->

## Final Remarks
It’s with no doubt the Emerging Markets had a stellar performance the past 2 decades. But what remains inherently  attached with these developing markets is: (i.) lack of proper oversight on market monitoring and supervision; (ii.) the lack of or inadequate liquidity in the market among other challenges.
In the coming posts I hope to dwell more on the performance of the LuSE and have a look at its peer exchanges in the region.


P.S: I used R statistical Computing Language for my analysis. For the data and the code,you can find them on [my GitHub account](https://github.com/ASimumba/LuSE_Data). Do check them out and run your own analysis.