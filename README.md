# CS416 Narrative Visualization Assignment
D3.js Narrative Visualization for CS416 Data Visualization 

# Project
This project is hosted live on Github Pages at .

# Introduction
This narrative visualization is an interactive slideshow which takes the user through the Yelp restaurant dataset. The dataset consists of the reviews and aggregated check-ins over time of numerous businesses located throughout various metropolitans across the globe but we'll only focus on a couple of states in the United States to reduce the computational complexity of the preprocessing of the dataset. This visualization focuses on the data from the United States which includes the following states: British Columbia, Colarado, Florida, Georgia, Massachusetts, Ohio, Texas and Washington.

## Visual Structure
This visualizations utilizes a static canvas of 1024x768 pixels, users should view the interactive visualization with a resolution of at least 1280x800 pixels to ensure optimal compatibility and ensure that the text and elements are at the right positions.

## Analysing the Dataset
This dataset is a huge dataset with a size of 10GB and to streamline preprocessing, we have only extracted restaurant checkins to between 100 to 500 and reduced the states to just 8 states. This is to ensure that the restaurants have a minimum amount of checkins as well as ensuring that the checkins are not too excessive and also to reduce the computational complexity.

## Visual Scenes
We provided a coherent look for the interactive visualization using CSS and FullPage.js. Each page is transitioned similar to a slideshow and text elements are consistent across the slides. We also provided a navigation bar for users to skip between various slides and simple tooltips are triggered when the user mouse overs the navigation bar area.

## Annotations
We have utilized annotations and triggers are used to change the hidden parameter of the annotation. The Line Chart Visualization has an initial state of the hidden parameter which controls the display of the annotations set to false. As a user uses the brush bar to zoom on specific timelines, this will trigger changes to the line chart's horizontal axis, it will activate this hidden parameter. Also, the annotation will revert back to the default state when the user resets the brush bars.

## Parameters and Triggers
Both parameters and triggers are used in the line chart. We have parameters set for each state. These parameters are updated as we mouse over the line chart, providing the user with a real-time udpate of the amount of check-ins in a specified time. Another parameter is the brush bar below the line chart, This bar allows the user to zoom into the data to show a closer look of the data. As a user uses the brush bar to zoom on specific timelines, this will trigger changes to the line chart's horizontal axis to be updated to the selected section of the brush bar and this is proportional to the horizontal axis of the line chart

# Reference Materials
## Line Chart
+ [https://gist.github.com/DStruths/9c042e3a6b66048b5bd4](https://gist.github.com/DStruths/9c042e3a6b66048b5bd4)