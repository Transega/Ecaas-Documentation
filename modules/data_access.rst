########################
Data Processing & Access
########################

After Data is collected and submitted to the servers from the mobile application by the Enumerators,
Data pipeline has already been set to establish the quality of data and flag out data that may be invalid.
This is done by some automated scripts dedicated in assisting the process to be as efficient as possible as well as 
replicable accross different areas. 

*************
Data Cleaning
*************

In order to have good quaity data the automation process of data cleaning considers looking at points collected that fall outside the Assigned
areas of interest for the enumerator, Geographical location details of less accuracy *(> 10m)*, fabricated photographs during farm visits and reported 
weight of harvest that is an outlier or a scenario where the dry harvest is more than the wet harvest.

However, the process is not complete yet, as more data cleaning needs to done by looking at the farm boundaries by human eye in this case,
a Geospatial expert to accertain the location of the data points and also look into the feasibility of using this data to 
train machine learning models.

Given the importance this exercise the data collected by the Enumerators were subjuected to primary and secondary phases of data cleaning, 
with the primary stage being the automated scripts while the secondary phase, being use of a Geospatial tool by a Geospatial Expert in 
cleaning the data.

During this phase the following activities took place;

i. Ensure the data has the correct map projection(s) 

ii. Checking polygons if then fall within farm boundaries.
    *This was done by visualizing the data on a GIS tool, and having satellite imagery as the basemap.*

iii. Editing polygons they may have inconsistenties with farm boundaries by looking at the base map.

iv. Move the points that may have been collected but due to some reasons they have offsets to the farms 

v. Check for duplicate polygons

vi. Check for overlapping polygons


***************
Info about Data
***************




***********
Data Access
***********

The datasets are archived by PULA, they are free and can be downloaded on the following links;

PULA is open and committed to further engagements on data collection, product development as well as offering insurance 
products to small holder farmers either through respective authories, farm co-perations and/or individual farmers.



