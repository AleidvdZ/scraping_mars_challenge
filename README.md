# scraping_mars_challenge <br>
### Module 11 Challenge

## About
This challenge is to demonstrate web data scraping from two different web sites using Splinter and Beautiful Soup.  The deliverables are the following:

Deliverable 1: Scrape titles and preview text from Mars news articles.

from: https://static.bc-edx.com/data/web/mars_news/index.html 

Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

from https://static.bc-edx.com/data/web/mars_facts/temperature.html 

## Process and Resources

### Timeline

0718 Started and completed Deliverable 1 without any external input.  Used resources from Module 11 in class demos and practice assignments.

0718 Started Deliverable 2 but got stuck on for loops to extract header vs. table values

0720 Successfully scraped and assembled data into a Pandas DataFrame using one key resource (see link below)

0720 Completed code for first two analysis question

0721 Completed part 2 analysis with no issues.  Used previous Pandas modules to remind of syntax for analysis and graphing.

### Links used:

None for Deliverable 1

Link for BeautifulSoup scraping of header from rows: https://www.youtube.com/watch?v=G8ZJwhOsmTw&ab_channel=Learnerea

No additional specific resources, just reminders on how to set up some Pandas syntax from previous classes and support sites.

## Examples

None for Deliverable 1; Output is in Jupyter Notebook part_1_mars_news.ipynb

### Deliverable 2
<img width="396" alt="mars_weather_df" src="https://github.com/AleidvdZ/scraping_mars_challenge/assets/131220504/fd2eb47f-ee56-4d48-991f-1da96c7955c1">
<br>

Plots are included in Jupyter Notebook part_2_mars_weather.ipynb and match the results shared in starter code.

## Analysis for Deliverable 2 (also in Jupyter Notebook)

Data Analysis - Aleid van der Zel
Below are the answers to the question posed at the beginning of the :

How many months exist on Mars?
Since the column definition describes "month: the Martian month", the data was analyzed using a groupby on the month along with a count of days by that group. This provides two answers - the number of Martian months, which is 12, and also the number of days that data was recorded on during each month (which vary).

How many Martian (and not Earth) days worth of data exist in the scraped dataset?
The instructions describe "sol" as the number of days Curiosity has been on Mars and it increments in the column. Completing a count of the number of data rows (unique days) in the "sol" column. There were 1867 days recorded.

What are the coldest and the warmest months on Mars (at the location of Curiosity)?
The coldest month on Mars (at the location of Curiosity) is Month 3 (average min temp (oC) = -83.307292)
The warmest month on Mars (at the location of Curiosity) is Month 8 (average min temp (oC) = -68.382979)

Which months have the lowest and the highest atmospheric pressure on Mars?
The lowest atmospheric pressure on Mars (at the location of Curiosity) is Month 6 (745.054422)
The lowest atmospheric pressure on Mars (at the location of Curiosity) is Month 9 (913.305970)

About how many terrestrial (Earth) days exist in a Martian year?
There are three distinct peaks from which and estimate of "seasons" can be made.
The first peak to peak is approximately 750 - 150 = 600 days
The second peak to peak is approximately 1425 - 750, or 675 days (provided in starter data)
This would result in an average of approximately 638 days (visually) <br?
By sorting by min temp in descending order a little better estimation can be made (it is an estimate because data was not recorded on every terrestrial day within a martian month).
day 1384 = -66
day 716 = -65 which is about 648 days to the final peak
day 129 = -63 which is about 587 days to the second peak
This still gives an estimated average of around 617 days

Both of these estimates are less than the internet search of 687 Earth days = a Mars year (https://mars.nasa.gov/all-about-mars/facts/mars-year/#:~:text=This%20is%20the%20vernal%20equinox,year%20is%20687%20Earth%20days).

## Installing

Jupyter Notebook

Splinter

Beautiful Soup

Pandas

Matplotlib

## Contributing

Solo Challenge - Aleid van der Zel


