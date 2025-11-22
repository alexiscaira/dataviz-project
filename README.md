# Data Visualization Project

## Background

Many claim they have spotted _Bigfoot_ (also commonly referred to as _Sasquatch_,) a large hairy man-like beast that often frequents the woods of North America. Bigfoot reports have dated back to before the written word, with earliest traces being found in native american folklore, but what about the claims of today? How does Bigfoot fit into the modern world and into American culture? Or is Bigfoot lost to time as sighting die out in the age of modern media and smart phone video? For this project, we'll be taking a look at a modern data set from the [Bigfoot Field Researchers Organization (BFRO)](https://www.bfro.net/GDB/) to spot trends visualize data to answer our questions about modern Bigfoot sightings across the United States from the 1990's and on. We'll try to answer if various weather conditions impact the number of reports claimed, if one type of weather condition corresponds with more reports than others, and also investigate what part of the United States has the most reports by state. 

## Data Used

The data used for this project is from [Bigfoot Field Researchers Organization (BFRO)](https://www.bfro.net/GDB/) data set and includes reports from members across the United States. Because the original data set is very large in size (5000+ rows, 10.99 MB), it was cleaned it a second time (as the original was cleaned once prior, found at: https://data.world/timothyrenner/bfro-sightings-data) and removed the larger columns we would not be using (index, observed) and any rows that did not contain values for weather conditions (temperature, pressure, etc.) which allows me to keep the spread of data in terms of place and time. This allows the data to be unified and more normalized to better view trends.

## Approach

For this process, we started with sketches to outline ideas of visualizations that users could interact with. The focus here was finding something that was both visually engaging but also understandable for users to see correlations and trends. 

![sketch iteration alexis](https://github.com/user-attachments/assets/7a131538-a454-4a05-a123-36740eb498c5)

In the above sketches, we've outlined some ideas of how users can interact with the chart to change the type of relation they are looking at. This includes toggles and drop down menus, which is standard for web interfaces and provide a minimal learning curve to have users start to use the visualization. The multiple types of interactions allow users to see how each type would change the total, since the y axis is the number of reports and should stay the same scale across graphics.

## Iterations
My first round of iteration included loading in the data, followed by a second iteration which was a scatterplot using two points in the set.
[![image](https://github.com/user-attachments/assets/b1fb0c70-0922-480f-964b-5e03f52ceb7d)](https://vizhub.com/alexiscaira/7f68f7b51f354021930fe9596dc14685)

These initial steps allowed us to get acclimatized to the set and figure out a direction for the project. By the fourth week, we used two relevant points from the data and added axis labels. 

[![image](https://github.com/user-attachments/assets/6d233b6c-6904-4f0a-9691-f7f0a0109030)](https://vizhub.com/alexiscaira/a39e7ee4ad4e4629bd232221d1213249)

The next step was integrating the bar charts to replace the scatter plots in the data to better match the sketches made.
[![image](https://github.com/user-attachments/assets/1abd463a-1dfd-4828-b08b-c2222e73a3d0)](https://vizhub.com/alexiscaira/3d91add8f7ad432aa264ccd1328783ea)

The following week, we added a toggle and drop-down integration and allowed users to change the type of weather or variable they were looking at. This was a particularly important step as this allowed the axis name, titles, and labels to be dynamic based on the state.

[![image](https://github.com/user-attachments/assets/bcfe7bf9-d979-419b-95bd-b08897bad7b9)](https://vizhub.com/alexiscaira/2b5047c1ad7e48799ba400d0ec7ad0a5)

For week seven, a few things were added including the bar chart coloring by type, and pickers to choose to view by season or type of precipitation. There was also a new tool tip to show the total segment as well that matches the theme.

[![week 7 demo mov](https://github.com/user-attachments/assets/cc41285d-a3c0-4581-a6cf-8edff06af33c)](https://vizhub.com/alexiscaira/b2322c7158ea424d9157c202aa31b435?mode=embed)

This flowed nicely into the polish part of the graph section of the visualization, which was adding animation with an on-hover effect when the user went over a type of precipitation on the bar chart, along with adding a trend-line for the graphs to help users better see the general shape of the data.

[![week 9 demo mov](https://github.com/user-attachments/assets/8c8fde0c-5f88-4537-a217-c526b96a95c9)](https://vizhub.com/alexiscaira/88a741e7705541198eabb2ded7bc4085?mode=embed)

For the map, we have a map with the geohash data integrated along with a toggle for both view states so you can go back and forth from the graph to this view, and then added a zoom in and zoom out feature that also pans back to the original location the user was on. There is also a tool tip integrated to read specific location reports for a point on the map, which adds a fun layer of interactivity. 

[![image](https://github.com/user-attachments/assets/fea52dcc-b708-42eb-8273-9136bb79b494)](https://vizhub.com/alexiscaira/7906aefd34674c4eaef72dce8c6c60ca?mode=embed)

For the polish iteration, pictured below, the colors were updated to lean more into the forest feel. The map also was updated to now have data points as tiny pine trees to also blend into the theme a bit more. There was also some resize work done to now fit the user's browser window to fill it out better and provide more space to interact with. 

## Final Product
The final, put together product can be found [here)](https://vizhub.com/alexiscaira/7906aefd34674c4eaef72dce8c6c60ca?mode=embed) where you can interact with both the graph and the maps and investigate the trends.  
<img width="1423" height="735" alt="Screenshot 2025-11-21 at 9 54 58 PM" src="https://github.com/user-attachments/assets/cdad01a0-7f7e-40be-be0e-19792aedd63b" />
<img width="1421" height="734" alt="Screenshot 2025-11-21 at 9 54 41 PM" src="https://github.com/user-attachments/assets/4c350065-4dec-4e82-8efb-44a8ea6f5d31" />
<img width="1419" height="734" alt="Screenshot 2025-11-21 at 9 54 32 PM" src="https://github.com/user-attachments/assets/7bd24bd8-c5a3-40f6-ad61-d132418400a5" />

## Findings

From our graphs, it's clear that Bigfoot sightings skew based on the type of weather reported. Across the temperature averages, there was no strong skew one way or another for generally more reported temperatures for sightings, which makes sense given the diverse climates across the United States. For dew point, there was a larger right skew towards more sightings at higher dew points. Humidity saw a bell-curve adjacent form for the distribution, with more sightings towards the 0.65 to 0.9 percent range. Cloud cover saw a strong skew of less cloudy days reporting more sightings than other coverage percentages. For pressure, the distribution of reports was close to a bell curve, which was unexpected to see in the data and a fun surprise. The UV index and moon phase did not have a large skew one way or another for the number of reports, which seems like a less impactful factor compared to the other data with stronger trends. For visibility, the higher visibility days had more sightings than lower days. For wind speed, more sightings were reported on less windy days than the windier days. 

When looking at the map, a few areas across the United States stand out with more reports than others including the pacific northwest and eastern United States. There was a surprising amount reported in Florida and Ohio, which was interesting given that the traditional Bigfoot folklore does not mention those areas commonly.  There were few in the western United States, which also could overlap with the population density for the region as well as the great plain region would be less populated than the larger major cities which would have more people to report sightings. Further future work here could investigate the density against the sightings on the map to confirm these assertions further. 

## Takeaways
This project was a fun exploration into a topic that was a bit on the sillier side but still provided a great learning value as we iterated over the few weeks and better familiarized ourselves with building out data visualizations that users can use and understand. Given a dataset that was very dense and there were so many attributes to work with, it was valuable to do the initial work to sketch and iterate to see how best to fit the data and let things come naturally to create something that really helps give a holistic view to such a broad range. 
