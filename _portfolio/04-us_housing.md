---
title: "US Housing Market"
excerpt: "Create an interactive dashboard of the US Housing Market from 2002 to 2022. I then analyse two large spikes in sales in 2016 and 2021.<br/><center><img src='https://github.com/SJackson123/SJackson.github.io/blob/master/images/us_housing/us_housing_4.png?raw=true' width='640px'></center>"
collection: portfolio
---

<p align="justify">In this project, I used Excel to analyse US Housing Market Data from 2002 to 2022. Given the dataset was over 1 million lines (limit of an excel file), I used the Power Query editor to load the data into Excel’s data model, preventing any data loss. Additionally, Power Query was useful for transforming my data. I wanted to calculate month over month performance in sales, however, Excel would automatically calculate month over month sales starting each year and return a blank value for January. You can get around this problem by creating a new column with the format ‘YYYYMM’.</p>

## Why is there a spike in sales in December 2016 and August 2021?

<p align="center">
  <img src="https://github.com/SJackson123/SJackson.github.io/blob/master/images/us_housing/us_housing_3.png?raw=true?raw=true"
 alt="EU Trend Over Time" width="1200px"/>
</p>

<p align="justify">Both spikes occur from an abnormally large sale amount. In December 2016 there were 9 high rise apartments blocks sold in Stamford, Connecticut. According to the dataset each block was sold for $395,000,000. This seems too large. </p>

<p align="justify">Looking on Zillow.com, each apartment block typically contains around 196 units, with individual prices ranging from $248,000 to $412,000 as of 2024. If we assume a standard block size of 196 apartments across all 9 blocks, this totals 1,764 apartments.</p>

<p align="justify">Dividing the reported sales price of $395,000,000 by the total amount of apartments, we get an average price of $223,900 per apartment. Considering inflation and the current housing market in Stamford <sup>[1]</sup>, this price aligns more closely with my pricing expectations. This demonstrates that the reported sale is likely the sales amount for all 9 apartment blocks sold together.</p>

<p align="justify">While the spike in 2016 can be rationalised, the spike in August 2021 seems to be an error. This instance involves the sale of 4 properties on a single plot, with a reported sale value of $5 billion. This figure seems implausible since one of the properties is available for rent now at $1700 per month.</p>

[1]: https://www.redfin.com/city/18605/CT/Stamford/housing-market
