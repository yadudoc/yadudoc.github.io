---
layout: post
title: "First month trading bitcoin"
description: ""
category: ""
tags: [Bitcoin, Trading]
---
{% include JB/setup %}

I am not going to write about the risks and potential of Bitcoin, topics which have been
debated over in great length. Instead I would write about my first month as a newly minted
investor. This is the first time I've invested money in a tradeable good, and I would like
to note my mistakes and my learnings.

Yes, I made the newbie mistake of watching the charts after my Bitcoins arrived in the wallet
for price drops and panic sold. "Sell high, buy low" is not as easy to follow through with
money and emotions involved. What worries me the most is that the price of bitcoin at this point
is very speculative. I do not know if it is even possible to estimate the intrinsic value of bitcoin,
and trade purely on fundamentals, especially at the timescale of weeks/months.

With the wildly speculative and volatile nature of bitcoin, I think that automated strategies
and bots would fare better than a trader. The bitcoin market is active 24/7 and just keeping up
with the market would place considerable strain on a trader looking to maximise time in the market.

What I've ended up doing is write tests for different quantitative strategies. Here's my repo
on some simple scripts which backtest a few simple EMA cross strategies : [Number6 repo](https://github.com/yadudoc/Number6)
The backtests are very simple and make several assumptions such as buy/sell at open/close values
of hourly candles, no crosschecks across exchanges and arbitrary buy/sell threshold. <br />

Here's a simulation result showing over 1M USD generated from 5K USD in the span of a year.

    Results from running a simulation with $5000 USD with :
    Starting date :  2012-12-31 16:00:00
    Ending date   :  2013-12-16 05:00:00
    
    Simulation on 1 hour candles from MtGox.
     
    And basic buy threshold set to 1% of price, and sell threshold set to 3%
    
    Format : EMA1, EMA2, EMA3, Final sum in USD
     
    10, 27, 29, 1095964.1741853813
    4,  6,  10, 1038221.2753517051
    9,  27, 29, 1007524.4618898276
    9,  28, 29, 978802.05582687503
    1,  2,  3,  963086.42278712604
    9,  26, 29, 959511.73509285843
    10, 25, 32, 950532.6488902343
    10, 26, 32, 949953.92246836261
    9,  25, 29, 948698.65668256988
    10, 24, 32, 943597.0524466671