---
name: Final Project Group 8
tools: [Python, HTML]
description: This is the final project for group 8
---


# Final Project Link

Here is the [Workbook](https://mybinder.org/v2/gh/3nikolov/3nikolov.github.io/5b219d5b691643e049f1ffe7103001d8f6ec1808?urlpath=lab%2Ftree%2Fpython_notebooks%2Fis445_finalproject.ipynb)


## Summaries of the Plots

Note: To run our visualizations, the user needs to play the entire notebook. Our visualizations' interactivity component is supported with ipywidgets, and as such it will not automatically show the visualizations unless it is ran through manually. 

For our first interactive visualization, we created a correlation matrix heat map to identify quantifiable relationships across each city and the varying strengths city-to-city relationships have. All the cities in the dataset (Boston, Chicago, Cleveland, Denver, Houston, Los Angeles, Miami, New York City, San Francisco, and Seattle) are listed on the X and Y axes, and each city is compared to all the other cities. With this visualization, we can identify cities with the strongest and weakest relationships based on how high or low the correlation values are on the right side using the 'Correlation Values' legend. The lighter the color of each box, the weaker the relationship between the two cities and the darker the color is for each box, the stronger the relationship is between the two cities. Users get the option to select a sequential colormap to visualize the relationships based on personal preferences and to accommodate for the fact that we wanted our light-to-dark scale to be very uniform, which meant choosing color palettes based on a gradient rather than color palettes that used multiple colors. The final two graphs that are listed side by side beneath the correlation matrix graph was created to visualize more detail-oriented insights on a city-by-city basis. Users get the option to select a city (or multiple cities) of their choice and view a box plot on the left which illustrates the upper and lower quartiles, and the median for gas prices on a dollars per gallon level. The points sometimes above and below the boxes are outliers. The stacked line graph on the right visualizes the trends of the dollars per gallon cost for the selected city over time from 2000 to present day. Users can go city-by-city and compare and contrast the rates over time using these two interactive visualizations while getting a more detail-oriented analysis of the city's trends in comparison to the others.




