# Life Expectancy and GDP

The purpose of this project is to analyze data on GDP and life expectancy from the World Health Organization and the World Bank to try and identify the relationship between the GDP and life expectancy of six countries.


## Data Collection

Files : `life_expectancy`

For my data mining I used two sources: 
- GDP Source [World Bank](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD) 
- Life expectancy Data Source [World Health Organization](https://apps.who.int/gho/data/node.main.688)


## EDA

###  Exploring the species data a little more in depth

There are six countries, Chile, China, Germany, Mexico, the US, and Zimbabwe represented in the data. Looking over the data, there are inconsistencies with the column names. Life expectancy at birth (years) is descriptive so changed column name to LEABY.


### Exploratory Plots

Analyzing the data after the initial exploration.

The plot below shows the distribution of GDP. The distribution of GDP in the data is very right skewed where most of the values are on the left-hand side.

![chart 1](https://user-images.githubusercontent.com/26355917/146969373-2d0feaa7-e5c8-4b26-8ceb-1bb4f7056e95.png)

Next, examined the distribution of LEABY. The distribution of LEABY in the data is very left skewed where most of the values are on the right-hand side. This is almost the opposite of what was observed in the GDP column.

![chart 2](https://user-images.githubusercontent.com/26355917/146969775-593d5cc2-f849-4576-806f-ef288c561ccf.png)

Breaking up the data by countries, to find the average LEABY and GDP by country. Examining the Life Expectancy and all of the countries except for Zimbabwe have values in the mid-to-high 70s. This probably explains the skew in the distribution from before!

![chart 3](https://user-images.githubusercontent.com/26355917/146970183-acd0cab5-daee-42c3-9f1d-228754a072b5.png)

For the average GDP by Country it seems that the US has a much higher value compared to the rest of the countries. In this bar plot, Zimbabwe is not even visible where Chile is just barely seen. In comparison the USA has a huge GDP compared to the rest. China, Germany and Mexico seem to be relatively close in figures.

![chart 4](https://user-images.githubusercontent.com/26355917/146970420-79ea3aa9-fefc-4b16-8d57-c970fe89e164.png)

Comparing data is to visualize the distributions of each and to look for patterns in the shapes. Below, country is on the x-axis and the distribution of numeric columns : GDP and LEABY are on the y axis. In the GDP plot on the left, China and the US have a relatively wide range, where Zimbabwe, Chile, and Mexico have shorter ranges. In the LEABY plot, many of the countries have shorter ranges except for Zimbabwe which has a range spanning from the high 30s to the high 60s.

![chart 5](https://user-images.githubusercontent.com/26355917/146970935-739bfa2e-aabc-4971-9f9f-02b6fae01213.png)

Showing distributions using swarm plot, as they can be used to complement the box and violin plots. First the stand alone swarm plot is shown and then overlayed on top of a violin plot. 

In the case of of the `GDP` plot on the left, Chile and Zimbabwe have a vertical line of dots that illustrate the number of data points that fall around their values. This detail would have been lost in the box plot, unless the reader is very adept at data visualizations. 

![Screen Shot 2021-12-21 at 12 17 02 PM](https://user-images.githubusercontent.com/26355917/146971634-bc549acf-293b-4526-a987-a9069ac3fb52.png)

![Screen Shot 2021-12-21 at 12 18 07 PM](https://user-images.githubusercontent.com/26355917/146971780-f2a98e0e-0565-4890-9e2f-c66d9ddb4a01.png)

Exploring `GDP` and `LEABY` over the years through line charts. Below the countries are separated by colors and one can see that the US and China have seen substantial gains between 2000-2015. China went from less than a quarter trillion dollars to one trillion dollars in the time span. The rest of the countries did not see increases in this magnitude.

![Screen Shot 2021-12-21 at 12 19 47 PM](https://user-images.githubusercontent.com/26355917/146972001-374aae7c-f211-4eb0-b090-7decc318c87a.png)

Examining different aspects with faceted line charts by Country. In the individual plots, each country has their own y axis, which makes it easier to compare the shape of their GDP over the years without the same scale. In the chart above, the other country's GDP growth looked modest compared to China and the US, but all of the countries did experience growth from the year 2000.

![Screen Shot 2021-12-21 at 12 24 46 PM](https://user-images.githubusercontent.com/26355917/146972580-e5d4f45f-fb9c-4255-9023-3da6fed4fff8.png)

The charts below show life expectancy over the years. It is evident that every country has been increasing their life expectancy, but Zimbabwe has seen the greatest increase after a bit of a dip around 2004.

![Screen Shot 2021-12-21 at 12 35 31 PM](https://user-images.githubusercontent.com/26355917/146973928-2d328502-ed43-44b8-8ab1-326e7cec7571.png)

After breaking out life expectancy by country. It is apparent that Chile, and Mexico seemed to have dips in their life expectancy around the same time which could be looked into further. Also the seemingly linear changes were in reality was not as smooth for some of the countries.

![Screen Shot 2021-12-21 at 12 37 16 PM](https://user-images.githubusercontent.com/26355917/146974148-e58c4e40-cc43-4def-9ea1-1be79fe19e6f.png)

Exploring the relationship between GDP and LEABY. In the chart below, it looks like the previous charts where GDP for Zimbabwe is staying flat, while their life expectancy is going up. For the other countries they seem to exhibit a rise in life expectancy as GDP goes up. The US and China seem to have very similar slopes in their relationship between GDP and life expectancy.

![Screen Shot 2021-12-21 at 12 38 18 PM](https://user-images.githubusercontent.com/26355917/146974269-4aa9989f-624b-400d-8634-925e09ce3d9f.png)

Looking at the individual countries, most countries like the US, Mexico and Zimbabwe have linear relationships between GDP and life expectancy. China on the other hand has a slightly exponential curve, and Chile's looks a bit logarithmic. In general though one can see an increase in GDP and life expectancy, exhibiting a positive correlation.

![Screen Shot 2021-12-21 at 12 38 52 PM](https://user-images.githubusercontent.com/26355917/146974338-9f5a0909-794a-498c-9ec2-6877561d3612.png)




### Conclusions

- The life expectancy increased over time in the six nations, with Zimbabwe having the greatest increase.
- GDP has increased for all countries in our list, especially for China.
- There is a positive correlation between GDP and life expectancy for countries in our list.
- Average life expectancy was between mid to high 70s for the countries except for Zimbabwe which was 50.
- The life expectancy had a left skew, or most of the observations were on the right side.
