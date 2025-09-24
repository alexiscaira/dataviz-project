# Data Visualization Project

## Data

The data I propose to visualize for my project is from [Bigfoot Field Researchers Organization (BFRO)](https://www.bfro.net/GDB/) data set and includes reports from members across America. Because the orginal data set is very large in size (5000+ rows, 10.99 MB), I went ahead and cleaned it a second time (as the orginial was cleaned once prior) and removed the larger columns I would not be using (index, observed) and any rows that did not contain values for weather conditions (temp, pressure, etc.) which allows me to keep the spread of data in terms of place and time.

https://data.world/timothyrenner/bfro-sightings-data

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

- How does various weather conditions impact the number of reports claimed? 
- Does one type of weather condtion correspond with more reports than others (aka- what does big foot like?)
- Are trends visible easily and the user can control what information is seen?
  
## Sketches
![sketch iteration alexis](https://github.com/user-attachments/assets/7a131538-a454-4a05-a123-36740eb498c5)
In the above sketches, I've outlined some ideas of how users can interact with the chart to change the type of relation they are looking at, likely by a drop down and toggles but I am exploring more ways to make this more fun. I don't think tool-tips would be partically exciting, but it would be nice to get some cross fades and animations going to really make it look nice. The multiple types of interactions allow users to see how each type would change the total, since the y axis is number of reports and should stay the same scale across graphics. For the bars, I also thought it would be fun to get an animation of something like leaves or snow falling when the user hovers over a type of precipitation. 

## Prototypes
My first round of iteration included [loading in the data](https://vizhub.com/alexiscaira/70933d6a9c7b470389d47af21262f796):
[![image](https://github.com/user-attachments/assets/7193c856-25c9-49c9-96b3-24971253d441)](https://vizhub.com/alexiscaira/70933d6a9c7b470389d47af21262f796)

My second round of iteration included [creating a scatter plot of two points in the data ](https://vizhub.com/alexiscaira/70933d6a9c7b470389d47af21262f796):
[![image](https://github.com/user-attachments/assets/b1fb0c70-0922-480f-964b-5e03f52ceb7d)](https://vizhub.com/alexiscaira/7f68f7b51f354021930fe9596dc14685)

My third round of iteration included [iterating on the scatter plot to use two points of relevent the data and add axis/labels](https://vizhub.com/alexiscaira/a39e7ee4ad4e4629bd232221d1213249):
[![image](https://github.com/user-attachments/assets/6d233b6c-6904-4f0a-9691-f7f0a0109030)](https://vizhub.com/alexiscaira/a39e7ee4ad4e4629bd232221d1213249)

Most recently, I went ahead and updated the data to use the clean/simplied data so more points can be used & added bar charts to match the sketches instead of a scatter plot. 

// TODO AC ADD in link

## Open Questions
For this project, I'm still exploring ways to show the states and showing everything in a wholistic picture, given that the histogram/bar chart would show the correlation the cleanest compared to just an overlay over the states displaying the data. Using the geo data would be fun, but I don't think it blends well to the weather angle I want to run at and just want to make sure I have enough to really build out a cool viz. 

## Milestones
Week 5: Updated the data to use the clean/simplied data so more points can be used & added bar charts to match the sketches instead of a scatter plot.

Week 6: Create a concept of state & enable users to change the type of data via a input source & update the graphs/axis label/title to reflect

Week 7: Split bars by perciptation type

Week 8: Add key for perciptation type

Week 9: Explore options for on-hover perciptation animation

Week 10: Add cross fade/animation for when chart changes (large unknown here - I've done this in Kotlin/Jetpack Compose but not in React Native)

Week 11: Add trend toggle and interaction state

Week 12: Display trend line on graph based on state and polish
