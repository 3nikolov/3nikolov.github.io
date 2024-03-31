---
name: Homework 8 Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/CongDistxSqFt.png
description: This is homework 8
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 8 Plots

Below are my plots for homework 8. 

The vegachart HTML tags to get to these plots look like so:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/YearxFloors.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/YearxFloors.json" style="width: 100%"></vegachart>


```
<vegachart schema-url="{{ site.baseurl }}/assets/json/CongDistxSqFt.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/CongDistxSqFt.json" style="width: 100%"></vegachart>



## Summaries of the Plots

Both of my plots use the "buildings.csv" dataset provided to us from the PrairieLearn homework 8 post. Both of my plots are also a departure from both of the plots I made in Homework 7, as I wasn't satisfied with the homework 7 plots enough to keep them for this homework assignment, so for both plots they use different X and Y encodings and present altogether different plots. 

### First Plot
My first plot is plotting the "Year Acquired" variable as the encoded X coded temporally against the "Total Floors" variable as the encoded Y coded quantitatively. The plot is coded as circle points using mark_circle and the color is coded as "Rep District", which then provides a sequential blue color map. I have provided a tooltip of Rep District, Year Acquired, and Total Floors and made it interactive that way as well as using a pan-zoom effect (you hover over the plot with your cursor to get this interactivity). I had to transform the "Year Acquired" variable in the code such that all cases where there was a row that contained a "Year Acquired" of the value 0 had to be dropped, because it doesn't make sense to include datapoints with a "year" of 0. I was interested in making this plot to look less at how floors change with time and more at the distribution of if later years had more floors. I included the Rep District as a color because it was my first time making a plot with a tooltip and I thought that different districts might have different distributions of floors depending on what year it was.

### Second Plot
My second plot is plotting the "Congressional District" variable called "Congress Dist" as the encoded X, coded quantitatively against the "Square Footage" variable as the encoded Y variable which was also coded quantitatively. The plot is a bar plot using the command mark_bar() and the color of the bars are the column "Usage Description". I made this plot to look at what Usage Descriptions have more Square Footage allotted to them, as well as to look at which Congressional Districts have what types of building usages associated with them. The highest bar in congressional district 7 has a lot of "business" or "unusual" types, as do congressional districts 10 and 13. Another one of the most common usages is "assembly" and/or "storage", and we can also see commonly "health care". If I had more time, I would have wanted to add a tooltip to this plot.

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/3nikolov/3nikolov.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/3nikolov/3nikolov.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>

