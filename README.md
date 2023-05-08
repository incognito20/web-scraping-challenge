
## Web-Scraping Challenge

### Summary

The Web-Scraping Challenge is a full web-scraping and data analysis project using data about Mars. It involves the identification of HTML elements on a page, identification of id and class attributes, and the application of this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. This data is then used and transformed in a Pandas dataframe for analysis in order to answer the provided questions in Part 2.

### File Information

part_1_mars_news.ipynb = The code required to complete Part 1 as described below.

part_2_mars_weather.ipynb = The code required to complete Part 2 as described below.

MarsWeatherData.csv = The dataframe output from Part 2 in csv format.


### Part 1

In Part 1 of this challenge the code scrapes titles and preview text from Mars News (https://static.bc-edx.com/data/web/mars_news/index.html).

The high level steps of the code are:

#Create a Beautiful Soup object and use it to extract text elements from the website.

#Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

#Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:

#Store all the dictionaries in a Python list.

#Print the list in your notebook



### Part 2

In Part 2 of this challenge the code uses automated browsing to visit the Mars Temperature Data website (https://static.bc-edx.com/data/web/mars_facts/temperature.html). It then scrapes data from the table and reproduces it for analysis in a Pandas data frame.

The high level steps of the code are:

<ol>
<li>Uses automated browsing to visit the Mars Temperature Data site and inspects the page to identify which elements to scrape.</li>

<li>Using a Beautiful Soup object it scrapes the data in the HTML table.</li>

<li>The scraped data is assembled into a Pandas DataFrame using the same heading as the table on the website.</li>
</ol>

***Colum Headings with Description:***
<ul>
<li>id: the identification number of a single transmission from the Curiosity rover</li>
<li>terrestrial_date: the date on Earth</li>
<li>sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars</li>
<li>ls: the solar longitude</li>
<li>month: the Martian month</li>
<li>min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)</li>
<li>pressure: The atmospheric pressure at Curiosity's location</li>
</ul>


***Using this dataset, the following questions were asked (with answers or pointers to answers):***
<ul>
<li>How many months exist on Mars?</li>
<li>*Determined in cell Part 2, cell 8.*</li>

<li>How many Martian (and not Earth) days worth of data exist in the scraped dataset?</li> 
<li>*1867 as determined in Part 2, cell 9.*</li>

<li>What are the coldest and the warmest months on Mars (at the location of Curiosity)?</li>
<li>*The third is the coldest and the eighth is the warmest month as determined in Part 2, cell 13 of the analysis.*</li>

<li>Which months have the lowest and the highest atmospheric pressure on Mars?</li> 
<li>*The sixth month is the lowest and the ninth month is the highest based on results in Part 2, cells 14 and 15.*</li>

<li>About how many terrestrial (Earth) days exist in a Martian year?</li> 
<li>*Using Part 2, cell 17 to visually measure from the plotted data it looks like the it is about 680 days.*</li>
</ul>

### Works Cited

Extraction of table data in part_2_mars_weather.ipynb was modeled after code found here: https://scrapfly.io/blog/how-to-scrape-tables-with-beautifulsoup/

