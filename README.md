# Analyzing White Wine Quality

In this Project, I explore a dataset containing information on over 4000 White Wines. I provide visualizations and explanations to support my belief that white wines with lower residual sugar are of better quality.

### Getting Started

To view the entire report, download [`white_wine_analysis.html`](https://raw.githubusercontent.com/ParthThakur/Analysing-White-Wine-quality/master/white_wine_analysis.html) and open it using a web browser.

The [white wine analysis.rmd`](https://github.com/ParthThakur/Analysing-White-Wine-quality/blob/master/white%20wine%20analysis.rmd) documents the entire process of exploration. To run this file, and render the report locally you need RStudio. The dataset used can be found [here](https://github.com/ParthThakur/Analysing-White-Wine-quality/blob/master/wineQualityWhites.csv)

### Built With

- RStudio



### Key insights from the Report

![plot_1](img\plot_1.png)

This plot represents a key finding in my report. That quality of the white wine is significantly correlated to its density and its alcohol content. These were the two of the strongest correlations to the quality. Density at -0.31 and alcohol at 0.44. 

In the box plot at the top, the downward trend in the density of the wine tells that quality of wine increases with a decrease in the density. I changed the limits on the y-axis to exclude the bottom 1% and the top 1% of the data to make it easier to see this trend. In the second boxplot, I see the relationship between alcohol content and quality. I can see an upward trend, however, there is a dip in alcohol content before it starts to rise again. 

This dip makes me believe that there is a certain threshold for alcohol percent before it starts to have a positive impact on quality. In fact, I am certain, that if alcohol content keeps on rising, quality will start to dip again as higher concentrations of alcohol impart a bitter taste to wines. 

![plot_2](img\plot_2.png)

In this plot, I see the relationship between the three most significant variables. Specifically, the relationship between density and alcohol, and residual sugar. I split the sugar values in two to better visualize the data. Wines with residual sugar less than 3g/dm<sup>3</sup> are “Low sugar”, and those with more than that are “High sugar”. 

These three variables show the highest amount of correlation. As alcohol content increases, residual sugar, and density decrease. This makes sense, as, during the fermentation process, sugar is converted to alcohol. Since sugar is a heavy compound and alcohol is very light, the density goes on decreasing. 

This relationship also helps us understand the age of the wine. The older the wine, the longer it is fermented, which gives it a high alcohol content and a lower density. Hence I can also say that older wines are of better quality. 

![plot_3](img\plot_3.png)

This plot shows the relationship between all our important variables. I have facet wrapped the plot based on the quality of the wine, and added some jitter to the scatter plot to make it easier to visualize the date.

The relationship between residual sugar and density is very clear in the plot. With all high sugar wines having a higher median density than low sugar wines. By looking at the color distribution of the points, I can also observe that great quality alcohols have the highest concentration of high alcohol wines, while poor quality alcohols have the highest concentration of high sugar-low alcohol wines.

Hence I can conclude that sweet wines are in fact not of great quality and that the quality of wines is determined mostly by its alcohol content, and by extension its density and age.