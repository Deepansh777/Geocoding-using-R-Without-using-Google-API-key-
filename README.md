# Geocoding-using-R-Without-using-Google-API-key


Geocoding is the process of determining geographic coordinates for place names, street addresses, and codes (e.g., zip codes). Many organizations use Google API to geocode as a part of the data cleaning process. Many students (just like me) who want to geocode, may not be comfortable in spending money out of their pocket to get the coordinates for 50 different locations. To overcome this issue, I have designed an R Program that performs web scraping to obtain the coordinates for desired locations. The web scraping was performed on the [Geoplaner](https://www.geoplaner.com/) website.

After obtaining the latitude and longitude, I used the ggplot2 library to plot those locations. I did not use the leaflet library because the map does not render once the notebook is uploaded on GitHub.

In R, there are 2 main libraries for geocoding that are:

- rvest
- RSelenium

rvest helps you to read an HTML page and extract elements from it. However, we cannot interact with java using the rvest library. RSelenium allows us to have a web browser that is controlled by our code. Since the Geoplaner website uses javascript so RSelenium was used primarily.

**-Deepansh Arora**
