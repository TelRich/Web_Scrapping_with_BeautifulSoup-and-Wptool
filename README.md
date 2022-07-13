# Web Scrapping with Beautiful Soup and Wptool API
This project is about listing the Top 100 Universities in Nigeria and gathering information about them. The first data was extracted with [BeautifuSoup](https://pypi.org/project/beautifulsoup4/) package, from [Webometric Ranking table of 2020](https://www.theabusites.com/webometrics-ranking-2019/). This data include the list of the schools with their ranking and world ranking.

The other data was extracted from each school wikipedia page, with the help of [Wptools API](https://pypi.org/project/wptools/). It includes information such chancellor and vice-chancellor of the school, if there is any. 

## Libraries/Package Required
- Requests 
- Pandas 
- BeautifulSoup
- os
- Wptools 
- Time
- JSON
- Numpy

## Summary 
The extraction from webometrics ranking using BeautifulSoup was successful.

While manually getting the urls of each school from wikipedia, some schools such as Federal University Kashere Gombe State, has no wikipedia page, while some school has wikipedia page but no infobox. Due to some schools not having the required information needed, the JSON data was extracted with NaN as default value.

Both datas from Beautilful soup extraction and wptools extraction was merged together and saved to a file top_100_universities_in_nigeria.csv