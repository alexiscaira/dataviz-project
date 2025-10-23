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
### Week 1
My first round of iteration included [loading in the data](https://vizhub.com/alexiscaira/70933d6a9c7b470389d47af21262f796):
[![image](https://github.com/user-attachments/assets/7193c856-25c9-49c9-96b3-24971253d441)](https://vizhub.com/alexiscaira/70933d6a9c7b470389d47af21262f796)

### Week 2
My second round of iteration included [creating a scatter plot of two points in the data ](https://vizhub.com/alexiscaira/70933d6a9c7b470389d47af21262f796):
[![image](https://github.com/user-attachments/assets/b1fb0c70-0922-480f-964b-5e03f52ceb7d)](https://vizhub.com/alexiscaira/7f68f7b51f354021930fe9596dc14685)

### Week 4
My third round of iteration included [iterating on the scatter plot to use two points of relevent the data and add axis/labels](https://vizhub.com/alexiscaira/a39e7ee4ad4e4629bd232221d1213249):
[![image](https://github.com/user-attachments/assets/6d233b6c-6904-4f0a-9691-f7f0a0109030)](https://vizhub.com/alexiscaira/a39e7ee4ad4e4629bd232221d1213249)

### Week 5
Most recently, I went ahead and updated the data to use the clean/simplied data so more points can be used & added bar charts to match the sketches instead of a scatter plot. 
[![image](https://github.com/user-attachments/assets/1abd463a-1dfd-4828-b08b-c2222e73a3d0)](https://vizhub.com/alexiscaira/3d91add8f7ad432aa264ccd1328783ea)

### Week Six
For week six, I went ahead and updated the viz to now toggle between the weather patterns. This included updating the data for the x-axis, titles, and the lables along with adding the drop down box. 
[![image](https://github.com/user-attachments/assets/bcfe7bf9-d979-419b-95bd-b08897bad7b9)](https://vizhub.com/alexiscaira/2b5047c1ad7e48799ba400d0ec7ad0a5)

### Week Seven
For week seven, a few things were added including the bar chart coloring by type, and pickers to choose to view by season or type of percipation. There's also a new tool tip to show the total segment as well that matches the theme. This week, I think that I might pivot my project a bit and add a second type of visual in the next few weeks to use a map and geohash data, since that would round out the data used. I plan to use the city and state as tool-tip data and add markers shaped like bigfoot. At that point, I would have used almost every data column in the CSV which will feel pretty rounded out.
[![week 7 demo mov](https://github.com/user-attachments/assets/cc41285d-a3c0-4581-a6cf-8edff06af33c)](https://vizhub.com/alexiscaira/b2322c7158ea424d9157c202aa31b435?mode=embed)

### Week Nine
For week nine, we now have a trend line that can be toggled on and off. We also have an on hover effect for rain and snow based on the bar you hover over (sorted by percipation type) which adds some fun pizzaz. 
[![week 9 demo mov](https://github.com/user-attachments/assets/8c8fde0c-5f88-4537-a217-c526b96a95c9)](https://vizhub.com/alexiscaira/88a741e7705541198eabb2ded7bc4085?mode=embed)

## Open Questions
For this project, I'm still exploring ways to show the states and showing everything in a wholistic picture, given that the histogram/bar chart would show the correlation the cleanest compared to just an overlay over the states displaying the data. Using the geo data would be fun, but I don't think it blends well to the weather angle I want to run at and just want to make sure I have enough to really build out a cool viz. 

## Milestones
~Week 5: Updated the data to use the clean/simplied data so more points can be used & added bar charts to match the sketches instead of a scatter plot.~

~Week 6: Create a concept of state & enable users to change the type of data via a input source & update the graphs/axis label/title to reflect~

~Week 7: Split bars by perciptation type/Add key for perciptation type~

~Week 9: Explore options for on-hover perciptation animation/Add trend toggle and display line~

Week 10: Add map and integrate geohash data

Week 11: Add markers shaped like bigfoots for area, Add tool tip on hover to show city/state data

Week 12: Polish and integrate vizes to let users choose the view they want to use
