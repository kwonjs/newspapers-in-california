# Distribution of Registered* Newspapers** in California by City/Neighborhood

### Motivations behind this mini-project

I stumbled upon the Library of Congress's "Chronicling America" database of all the newsppaers that had been recorded since 1690 and wanted to see if there was a way I could scrape the data and visualize the distribution of recorded newspapers still operating today (labeled as "current" in the database) in California by county and by city/neighborhood. I wanted to see if there were certain geographic areas within California where there was a dearth of local daily or monthly news, online or in print. 

_Note: In conducting this project, I had to assume some things: the database was comprehensive, most of the data in the database was up-to-date and correct (i.e. that the newspapers/news outlets labeled as "current" were still operating), and that the headquarter locations of these outlets were accurate._

<iframe seamless frameborder="0" src="https://public.tableau.com/views/NumberofRegisteredNewspapersperCountyinCA_15982398810650/Dashboard1?:embed=yes&:display_count=yes&:showVizHome=no" width = '900' height = '900'></iframe>

<iframe seamless frameborder="0" src="https://public.tableau.com/views/NumberofRegisteredNewspapersperCountyinCA/Dashboard2?:embed=yes&:display_count=yes&:showVizHome=no" width = '900' height = '900'></iframe> 

_Note: "Registered" means all current news sources documented in the Library of Congress's "Chronicling America." "Newspapers" are broadly defined to include **all** publications in print/online that occur daily/monthly/other frequency. Some newspapers (~10) are not included from the scraped data due to ambiguity in location or lack of location (because they might be online-only). Some publications in less-populated areas were lumped with more-populated locations nearby, so the location data of news publications in this map may  not be entirely accurate._ 

The data supporting this visualization is scraped from the Library of Congress's "Chronicling America" [database](https://chroniclingamerica.loc.gov/search/titles/results/?state=California&county=&city=&year1=1690&year2=2020&terms=&frequency=&language=&ethnicity=&labor=&material_type=&lccn=&rows=9996) and cleaned using Google Sheets.

### Additional tool(s) used:

* [City-to-County Finder](http://statsamerica.org/CityCountyFinder/Default.aspx) (California-specific, used for building the county-level map!)

### Limitations:

* Tableau failed to recognize some census-designated places where local news outlets/papers were located, so I had to label these papers instead at the nearest town over. 
* From a glance, Los Angeles looks like it has an overabundance of newspapers. Most of the newspapers within that bubble in the City/Neighborhood visualization, however, were local to specific neighborhoods within L.A. (i.e. City of Industry, Van Nuys, Brentwood, Woodland Hills etc.) but were grouped because Tableau didn't have the specificity to recognize individual neighborhoods within L.A. 

### Ideas for future data analyses:

* Showing the distribution of _daily_ currently registered newspapers by **city/neighborhood** or by **county**
* Showing the language distribution of newspapers by **city/neighborhood** or by **county** 
* Answering the questions "Where and why are there newspaper dearths in certain locations in California?"
* Answering the question "Which entities own the newspapers in California?"
