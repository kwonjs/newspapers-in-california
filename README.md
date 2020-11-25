# Distribution of Registered* Newspapers** in California by City/Neighborhood

### Motivations behind this mini-project

I stumbled upon the Library of Congress's "Chronicling America" database of all the newspapers that had been recorded since 1690 and wanted to see if there was a way I could scrape the data and visualize the distribution of recorded newspapers still operating today (labeled as "current" in the database) in California by county and by city/neighborhood. I wanted to see if there were certain geographic areas within California where there was a dearth of local daily or monthly news, online or in print. 

_Note: "Registered" means all current news sources documented in the Library of Congress's "Chronicling America." "Newspapers" are broadly defined to include **all** publications in print/online that occur daily/monthly/other frequency. Some newspapers (~10) are not included from the scraped data due to ambiguity in location or lack of location (because they might be online-only). Some publications in less-populated areas were lumped with more-populated locations nearby, so the location data of news publications in this map may  not be entirely accurate._ 

The data supporting this visualization is scraped from the Library of Congress's "Chronicling America" [database](https://chroniclingamerica.loc.gov/search/titles/results/?state=California&county=&city=&year1=1690&year2=2020&terms=&frequency=&language=&ethnicity=&labor=&material_type=&lccn=&rows=9996) and cleaned using Google Sheets.

#### By city/neighborhood

<iframe seamless frameborder="0" src="https://public.tableau.com/views/NumberofRegisteredNewspapersperCountyinCA/Dashboard2?:embed=yes&:display_count=yes&:showVizHome=no" width = '900' height = '900'></iframe> 

#### By county

<iframe seamless frameborder="0" src="https://public.tableau.com/views/NumberofRegisteredNewspapersperCountyinCA_15982398810650/Dashboard1?:embed=yes&:display_count=yes&:showVizHome=no" width = '900' height = '900'></iframe>

<iframe width="912" height="504" seamless frameborder="0" scrolling="no" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQzJw4WGnYGZIVPcaTobpwAIVdne7fUNpGSuDqQXQ2QrnLoj2SnhZ89JbE6EEpzYZf4MGT7GT7WBxYJ/pubchart?oid=1726472795&amp;format=interactive"></iframe>

### Additional tool(s) used in this project:

* [City-to-County Finder](http://statsamerica.org/CityCountyFinder/Default.aspx) (California-specific, used for building the county-level map!)
* [How to embed Tableau visualizations](https://san-wang.github.io/blog/Embed-Tableau-dashboard-into-github-page-post/) in github markdown pages

### Limitations:

* In conducting this project, I had to make many assumptions: the database was comprehensive, most of the data in the database was up-to-date and accurate (i.e. newspapers/news outlets labeled as "current" were actually still operating), and that the headquarter locations of these outlets were accurate. (_Edit: As of August 2020, this database has expanded from 9996 registered newspapers to 10,000+, and these visualizations don't take into account these added news outlets that might still be currently operating!_)
* News outlets/newspapers that were completely online and thus had no "city location" or physical headquarters weren't able to be visualized. There also were some news outlets that bordered California and Nevada (i.e. "North Lake Tahoe Bonanza" in Incline Village that weren't plotted). 
* Tableau failed to recognize some census-designated places where local news outlets/papers were located, so I had to label these papers instead at the nearest town over. 
* From a glance, Los Angeles looks like it has an overabundance of newspapers. Most of the newspapers within that bubble in the City/Neighborhood visualization, however, were local to specific neighborhoods within L.A. (i.e. City of Industry, Van Nuys, Brentwood, Woodland Hills etc.) but were grouped under "Los Angeles" because Tableau didn't have the specificity to recognize individual neighborhoods within L.A. 

### Ideas for future data analyses:

* Showing the distribution of _daily_ currently registered newspapers by **city/neighborhood** or by **county**
* Showing the language distribution of newspapers by **city/neighborhood** or by **county** 
* Answering the questions "Where and why are there newspaper dearths in certain locations in California?"
* Answering the question "Which entities own the newspapers in California?"

##### [Click here to see the dataset](https://docs.google.com/spreadsheets/d/e/2PACX-1vQzJw4WGnYGZIVPcaTobpwAIVdne7fUNpGSuDqQXQ2QrnLoj2SnhZ89JbE6EEpzYZf4MGT7GT7WBxYJ/pubhtml?gid=1348884363&single=true) used to create the above visualizations
