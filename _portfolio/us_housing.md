---
title: "US Housing Market"
excerpt: "Create an interactive dashboard of the US Housing Market from 2002 to 2022. I then analyse two large spikes in sales in 2016 and 2021.<br/><center><img src='https://github.com/SJackson123/SJackson.github.io/blob/master/images/us_housing/us_housing_4.png?raw=true' width='640px'></center>"
collection: portfolio
---

## Why is there a spike in sales in December 2016 and August 2021?

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/us_housing/us_housing_3.png?raw=true?raw=true"
 alt="EU Trend Over Time" width="1200px"/>
</p>

Both spikes occur from an abnormally large sale amount. In December 2016 there were 9 high rise apartments blocks sold in Stamford, Connecticut. According to the dataset each block was sold for $395,000,000. This seems too large. 

Looking on Zillow.com, each apartment block typically contains around 196 units, with individual prices ranging from $248,000 to $412,000 as of 2024. If we assume a standard block size of 196 apartments across all 9 blocks, this totals 1,764 apartments.

Dividing the reported sales price of $395,000,000 by the total amount of apartments, we get an average price of $223,900 per apartment. Considering inflation and the current housing market in Stamford <sup>[1]</sup>, this price aligns more closely with my pricing expectations. This demonstrates that the reported sale is likely the sales amount for all 9 apartment blocks sold together.

While the spike in 2016 can be rationalised, the spike in August 2021 seems to be an error. This instance involves the sale of 4 properties on a single plot, with a reported sale value of $5 billion. This figure seems implausible since one of the properties is available for rent now at $1700 per month.

[1]: https://www.redfin.com/city/18605/CT/Stamford/housing-market
