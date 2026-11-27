---
title: Free memory call option
date: 2026-11-27
description:
unlisted: false
tags:
rich: false
---
Apple sells a beefy Mac Studio with 512GB of unified memory for $22,299 USD. This might be interesting to you if you want to run LLMs local - or if you want a free [call option](https://en.wikipedia.org/wiki/Call_option) on the spot price of RAM.

You can order it today, but it doesn't deliver until March. And Apple's policy lets you refund it until 2 weeks after it delivers. Which means you get to lock in the price today, and you don't have to pay until March. 

Leveraging this trade doesn't even require your own capital: you can put it on a credit card and it won't charge your card until it delivers.

# Backtesting
Let's say you did this in March 2025 (when the first M3 Ultra Mac Studio 512GB was released). It listed for $9.5k, and say you received the order 3 months later in June. Memory prices remained stable during that time so you'd gain nothing, but you can just reset the expiry date on your call option by cancelling and placing the order again. 

If you kept doing this, eventually your option would coincide with the run-up in memory prices. At this point, the machine you take delivery of would have increased in value, but you still gain nothing because as long as Apple sells it for its list price of $9.5k, you can't resell it for higher. 

But in March 2026, memory prices got way too high and Apple was forced to pull the 512GB configuration. And at that point, there was finally true price discovery in the resale market: 

```widget mac-studio-resale
```

The price instantly jumped up from ~9.5k to $19.5k overnight. It peaked at 21k a couple months later until Apple announced a 512GB configuration for their new M5 Ultra Mac Studio, this time at a much higher price. 

So if memory prices continue their run-up, we might see a repeat of this. The resale value stays bounded by the retail price until Apple either hikes the price or pulls it altogether. Will the run-up happen? Who knows, but at least you won't lose money[^1]

There's a lot of nuance here I didn't capture (nor fully explore myself):
- resale discount (condition, eBay fees, taxes)
- liquidity in the resale market
- DRAM spot price vs contract price
- Apple policy (how many times can you cancel? is the price truly locked in? will it always take 3 months from order to delivery?)


# Sources 
1. eBay price history: https://www.ebay.com/sh/research?marketplace=EBAY-US&keywords=mac+studio+m3+ultra+512gb+1tb&dayRange=730&endDate=1795593600000&startDate=1732521600000&excludedListings=198337521903&excludedListings=298305896692&excludedListings=318130004206&excludedListings=389835681400&excludedListings=960037766129&offset=0&limit=50&tabName=SOLD&tz=America%2FLos_Angeles
2. DRAM spot price history: https://www.dramexchange.com/ (via Internet Archive)



[^1]: This whole thought experiment started because I wanted to buy it for running local inference while convincing myself that it's "a good investment"
