# Assignment - 4

## Dataset
This dataset contains reported incidents of crime (excluding murders) that occurred in the City of Chicago from 2001 to the present day, excluding the most recent seven days. The data is sourced from the Chicago Police Department's CLEAR (Citizen Law Enforcement Analysis and Reporting) system. To protect privacy, addresses are provided at the block level only, and specific locations are not disclosed. It's important to note that the preliminary crime classifications may be subject to change after further investigation, and errors are possible. The Chicago Police Department does not guarantee the accuracy, completeness, timeliness, or correct sequencing of the information, and it should not be used for comparing crime statistics over time. The dataset will be updated daily.

# Webpage

Following are the interactive visualizations

<img width="1447" alt="image" src="https://github.com/uic-cs424/assignment-4-black-hawks/assets/144352425/b6513cc5-0fcc-4479-9ed9-a5b551d6dac0">

## Task 
We did a basic setup, by setting up a python server and creating a basic template for visualizations. We preprocessed the data files to save different data for the respective visualizations.

## Visulisation - Top Left
We have used D3 to complete this task and utilized the visualizations from the previous tasks to make the single view/ multi linked visualizations. In the visualizations, a high level of interaction is maintained where we have different interaction mechanism such as filtering, mapping, aggregation etc. We have also ensured to avoid overplotting by using only top entries for a particular attribute that is chosen. We have added a drop down for selecting arrest/ crime and one more drop down for checking total crime counts/arrest/ not arrest information.

The primary visualization focuses on analyzing trends in crime counts and arrest rates over the years or across different districts. Users can select a specific year and district from dropdown menus, and a second dropdown allows them to choose attributes such as crime counts, arrests, or incidents where arrests were not made for analysis.This allows users to interact with the graph to display specific data subsets based on year, district, or crime attribute. This type of interactivity allows for a more detailed and customized analysis of the data presented.

Upon selecting the desired options, a combined bar chart and line chart are generated. This dual visualization aids in easily comparing actual crime counts and arrest rates for various years/districts, facilitating the identification of any anomalies or patterns. Additionally, a dotted chart has been incorporated to compare crime counts in the years before and after the onset of the COVID-19 pandemic. Hovering over the dots during recent years reveals tooltips displaying crime counts labeled and categorized into different time periods related to COVID-19 for quick analysis.
<img width="1199" alt="image" src="https://github.com/uic-cs424/assignment-4-black-hawks/assets/144352425/113eaa50-776c-46fa-a2b6-e07e07cdcd30">

If we see the overall trend with year and crime counts, it has been decreasing over the years. For the analysis of not arrested, there hasnt been a steep decrease over time, while for arrest there has been a steep decrease. For the districts, we can see that the district had the highest crime count, while the total no of arrests made were the highest for disctrict 11.0. The district 8.0 again has the highest count of not arrested incidents. 
<img width="1164" alt="image" src="https://github.com/uic-cs424/assignment-4-black-hawks/assets/144352425/acd067dc-5694-47f2-9ded-3be277841e18">


## Linked Visualization - Bottom Left

We have two radio buttons either to analyze by crime type/ district or to analyze  by year/crime type. Upon selecting the button reveals an additional visualization. We have created a linked visualization where we can analyze the Crime counts with Arrest Trends for Top Crimes Types.

When we select the crime type/district, we can select the attribute i.e crime count, arrest and not arrest to see the bar chart for a particular crime type. It shows the count of that particular crime type. If we select a particular bar, i.e crime type, it shows a dotted chart to show the count of that crime type among the top communities. The number indicates the crime count.Similarly, we can check the count of Arrested and Not arrested crimes also by selecting a different option from the dropdown. Additionally the color intensity indicates the count i.e the higher the intensity, the higher the count.
The interaction mechanism is such that clicking on a specific bar in the upper graph filters the data in the lower graph to display information related to the selected crime type. This linked interaction provides a detailed analysis of crime distribution and arrest trends within specific community areas.
<img width="802" alt="image" src="https://github.com/uic-cs424/assignment-4-black-hawks/assets/144352425/1bb0c796-a9a0-46e6-8dd5-9520b5f98535">
<img width="818" alt="image" src="https://github.com/uic-cs424/assignment-4-black-hawks/assets/144352425/32b5eb93-9ec4-4d2a-b2a0-6679190fb0fa">

The other visualization contains analysing the crime count using the year/crime type. The line chart shows the crime count by years, and on brushing/selecting a particular area, we can see the cumulative count of crimes i.e the no of crimes according to crime types with Arrest vs Non-Arrest Counts over those selected years in a stacked bar chart. In  the bar chart on the x axis we have the crime type, on y axis we have the number of crimes, and the green color indicates the Crimes with arrest=true and the red ones indicate the non arrested crimes. When we hover over a particular bar, we can see the summary in the form of a tooltip i.e the crime type, arrest and the count. 
These visualizations ensure we are covering the important information, and researchers can use this to derive some conclusion on the reason behind the crimes happening or the overall effectiveness.
With this analysis, we can see that theft and battery tops among the most occuring crime types, and also, for Narcotics Crime type the arrest rate has been really good, showing efficiency of the narcotics bureau in ensuring law.

<img width="962" alt="image" src="https://github.com/uic-cs424/assignment-4-black-hawks/assets/144352425/945f3876-769c-48be-b094-84f5e8081513">

## Spatial Multi Linked Visualization - Right Side

In the multi-linked spatial visualizations, we have developed a spatial map representing the top 10 primary crime types for an year. Drawing inspiration from a previous assignment, this map provides a visual representation of the occurrence of each crime type across various locations.

The interactivity is enhanced by incorporating features such as hovering and clicking on a specific crime type in a particular area on the map. Upon interaction, a corresponding line chart is displayed, offering insights into the distribution of the selected crime type across the top 10 districts. This line chart details the number of incidents in each district, facilitating a quick understanding of spatial patterns. We have linked the spatial with distrcits to find out how that which district has the highest records for that specific crime type. 

Further exploration is possible by selecting a specific district on the line chart, prompting the display of a comparative analysis between arrested and not arrested incidents for that particular district. This comparison is presented using a donut chart, providing a clear visualization of the arrest outcomes.


![ezgif-5-fb16abe562](https://github.com/uic-cs424/assignment-4-black-hawks/assets/144352425/fd946a1a-4f7b-452b-bee2-caeb9d39dbb0)

