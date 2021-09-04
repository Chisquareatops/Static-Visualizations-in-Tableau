# Static Visualizations in Tableau

## Repository Structure
- Forest vs GDP
	- forest_area_GDP.csv
	- Q1_Workbook
	- Forestation_v_GDP.png
- Fish Production
	- fish2.csv
	- Q2_Workbook
	- Global_Fish_Production.png
- README.md

## The Relationship Between Deforestation/Reforestation and National Wealth

### Data
World Bank DataBank 
30kb of data, 217 rows, 8 columns
percent of total land which is forested and per capita GDP in fixed 2010 USD for 217 countries for 4 years (2000, 2005, 2010, 2015)

Data has been cleaned since download.

### Discussion
To examine the relationship between national wealth and reforestation/deforestation, this visualization uses the percent change in forested land between 2000 and 2015.
In service of digestibility, the select visualization narrows the focus of the dataset to twenty countries: the ten wealthiest and the ten least wealthy. National GDP is depicted using a color scale from red (lowest GDP) to blue (highest GDP). Change in forested land is shown using a horizontal bar chart across the zero axis, where deforestation is a net negative change and reforestation is a net positive change.

This visualization allows us to see clearly that a relationship between wealth and reforestation/deforestation does exist, as wealthy countries are disproportionately represented on the right side of the axis. We also see that the richest country added almost as much forest as the poorest country lost, which is striking. This visualization also expresses some interesting information about wealth inequality through the relative scarcity of pinks, the appearance of dark blue in only two rows, and the fact that only nine total countries are shown in blue (meaning the tenth wealthiest country in the world still falls below the mean).

### Other Considerations
Other versions of this visualization set the midpoint of the color scale to the median GDP rather than the mean. Because wealth is so unevenly distributed that only a handful of countries lie above the mean, using the mean for the midpoint of the color scale causes most countries to be shown in extremely similar shades of red with only a few countries appearing in any shade of blue. When all 217 countries are shown, this makes it much more difficult to assimilate the information about GDP and obscures the relationship of interest. 

In this visualization, the view of the data was narrowed to a subset of countries in which wealthy and poor countries are equally represented. Using this view, the skewed color scale conveys some information about wealth inequality without obscuring meaning.


## Changes in Global Fish Production Over Time

### Data
World Bank DataBank 
2.4 kb, 56 rows, 6 columns
global capture fish production in metric tons ('Capture fisheries production (metric tons) [ER.FSH.CAPT.MT]') and total fish production in metric tons ('Total fisheries production (metric tons) [ER.FSH.PROD.MT]') for each year from 1960 to 2015, inclusive

Data has been cleaned since download.

### Discussion
This visualization depicts general trends in fish production over several decades. It clearly illustrates that the global increase in fish farming parallels the overall increase in global production, culminating in the crossover point in the mid-2010s when farming finally eclipses capture fishing (which had been relatively stagnant since the 1990s. It also illustrates some broad historical trends; for example, fish farming existed in the 1960s but was relatively unimportant on the global scale until the 1990s, a decade during which some important modern hatchery techniques began to spread rapidly around the world.

### Other Considerations
This dataset has in the past lacked informative indicators of marine health that could be reasonably tied to changes in fish production patterns. This may be change, as two potentially useful variables do exist: marine protected areas and fish species threatened. At this time this data slice was pulled from the DataBank interface, the marine protected areas field was empty and the fish species threatened field was new, with only one year of data.

The fish farming variable is derived by subtracting the capture fish production from the total fish production contained in the original dataset. Before deriving this variable, it was confirmed that the total production indicator included the entire volume of all aquatic species caught by a country for all commercial, recreational, industrial, and subsistence purposes. It explicitly includes harvest from wild sources and all kinds of fish farming. It was also confirmed that the capture fish production indicator includes the entire volume of aquatic species caught by a country for all of the same purposes. Therefore, it can be reasonably concluded that the difference between these indicators can be used to represent the production of farmed fish.
