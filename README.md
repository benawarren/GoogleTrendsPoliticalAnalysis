# Google Trends Partisan Conflict Analysis
In this repository, I use regression and time-series analysis to investigate the relationship between Google search trends and partisan conflict in the U.S. federal government. 

**Summary**

The Partisan Conflict Index is a useful tool that measures the level of partisan disagreement within the federal government, but it is worth asking whether trends in the general populace are associated with trends in the PCI. For example, using Google search data, might we find a link between the public searching certain terms and higher levels of partisan conflict?

I approach this question using two different methods. First, I use simple regression analysis to identify potential relationships between the search trends and the PCI, finding a statistically significant (negative) correlation between searches for "Democrat" and the conflict index. Then, I use time-series analysis to better understand the temporal relationship between searches for political/partisan terms and PCI.

**Data Sources:**
 - Partisan Conflict Index: The Federal Reserve Bank of Philadelphia publishes the [Partisan Conflict Index](https://www.philadelphiafed.org/surveys-and-data/real-time-data-research/partisan-conflict-index) monthly on its public website. The index "tracks the degree of political disagreement among U.S. politicians at the federal level" as measured by the frequency of articles from major newspapers like the Washington Post, New York Times, and the LA Times that report political disagreement in a given month. Data is available dating back to 1981, but in this analysis, I utilize data since 2004.

 - Google Trends: Google publishes a [data tool](https://trends.google.com/trends/explore?date=all&hl=en) that allows users to view, compare, and download data on the "search interest" of various terms since 2004. For this analysis, I downloaded monthly data sets for the general political terms "Senate", "Congress", "Government", and "Protest" and the partisan terms "Democrat" and "Republican," confining all search data to the United States.

**Guide to files**
 - MultiTimeline.csv: main data file with Google Trends and PCI data by Year and Month.
 - PartisanConflictAnalysis.Rmd: R Markdown file with analysis
 - PartisanConflictAnalysis.pdf: PDF of analysis for easier viewing (compiled from R Markdown)


