# Matplotlib-Visualize-data
 
Data scientists visualize data to understand it better. This can mean looking at the raw data, summary measures such as averages, or graphing the data. Graphs are a powerful means of viewing data, as we can discern moderately complex patterns quickly without needing to define mathematical summary measures.

epresenting data visually typically means graphing it. This is done to provide a fast qualitative assessment of our data, which can be useful for understanding results, finding outlier values, understanding how numbers are distributed, and so on.

While sometimes we know ahead of time what kind of graph will be most useful, other times we use graphs in an exploratory way. 

Graphs aren't limited to 2D scatter plots like those above, but can be used to explore other kinds of data, like proportions - shown through pie charts, stacked bar graphs - how data are spread - with histograms, box and whisker plots - and how two data sets differ. Often, when we're trying to understand raw data or results, we may experiment with different types of graphs until we come across one that explains the data in a visually intuitive way.

DataFrames provide a great way to explore and analyze tabular data, but sometimes a picture is worth a thousand rows and columns. The Matplotlib library provides the foundation for plotting data visualizations that can greatly enhance your ability to analyze the data.

We used the pyplot class from Matplotlib to plot the chart. This class provides a whole bunch of ways to improve the visual elements of the plot. For example, the following code:

1.Specifies the color of the bar chart.
2.Adds a title to the chart (so we know what it represents)
3.Adds labels to the X and Y (so we know which axis shows which data)
4.Adds a grid (to make it easier to determine the values for the bars)
5.Rotates the X markers (so we can read them)

## Histogram and  Pie chart
![image](https://user-images.githubusercontent.com/79583184/199757656-27332ce2-f68d-4163-bf01-6ed6544f6845.png)

## Data Distribution
![image](https://user-images.githubusercontent.com/79583184/199758043-c8c991a1-79a3-420e-93dd-12aef37d30ad.png)

## Measures of central tendency
To understand the distribution better, we can examine so-called measures of central tendency; which is a fancy way of describing statistics that represent the "middle" of the data. The goal of this is to try to find a "typical" value. Common ways to define the middle of the data include:

1.The mean: A simple average based on adding together all of the values in the sample set, and then dividing the total by the number of samples.
2.The median: The value in the middle of the range of all of the sample values.
3.The mode: The most commonly occuring value in the sample set.

Minimum:3.00
Mean:49.18
Median:49.50
Mode:50.00
Maximum:97.00

![image](https://user-images.githubusercontent.com/79583184/199759142-20c0b0e5-7933-4033-ad23-53f6ac44d6a2.png)

Another way to visualize the distribution of a variable is to use a box plot (sometimes called a box-and-whiskers plot). Let's create one for the grade data.

## Box Plot
![image](https://user-images.githubusercontent.com/79583184/199759482-25b3e5b4-b0d7-4c97-87d8-91ab7f5b954f.png)

The box plot shows the distribution of the grade values in a different format to the histogram. The box part of the plot shows where the inner two quartiles of the data reside - so in this case, half of the grades are between approximately 36 and 63. The whiskers extending from the box show the outer two quartiles; so the other half of the grades in this case are between 0 and 36 or 63 and 100. The line in the box indicates the median value.

For learning, it can be useful to combine histograms and box plots, with the box plot's orientation changed to align it with the histogram (in some ways, it can be helpful to think of the histogram as a "front elevation" view of the distribution, and the box plot as a "plan" view of the distribution from above.)
Minimum:3.00
Mean:49.18
Median:49.50
Mode:50.00
Maximum:97.00

![image](https://user-images.githubusercontent.com/79583184/199760381-bc0c77e6-c759-44db-852b-0d624a600c6f.png)

## Probability density function
All of the measurements of central tendency are right in the middle of the data distribution, which is symmetric with values becoming progressively lower in both directions from the middle.

To explore this distribution in more detail, you need to understand that statistics is fundamentally about taking samples of data and using probability functions to extrapolate information about the full population of data.

What does this mean? Samples refer to the data we have on hand - such as information about these 22 students' study habits and grades. The population refers to all possible data we could collect - such as every student's grades and study habits across every educational institution throughout the history of time. Usually we're interested in the population but it's simply not practical to collect all of that data. Instead, we need to try estimate what the population is like from the small amount of data (samples) that we have.

If we have enough samples, we can calculate something called a probability density function, which estimates the distribution of grades for the full population.

The pyplot class from Matplotlib provides a helpful plot function to show this density.

![image](https://user-images.githubusercontent.com/79583184/199760796-2f97255b-e131-463d-ad49-ccd40027ab7d.png)

As expected from the histogram of the sample, the density shows the characteristic "bell curve" of what statisticians call a normal distribution with the mean and mode at the center and symmetric tails.

## Summary

Here we have:

* Made graphs with matplotlib
* Seen how to customise these graphs
* Calculated basic statistics, such as medians
* Looked at the spread of data using box plots and histograms
* Learned about samples vs populations
* Estimated what the population of graphse might look like from a sample of grades.




