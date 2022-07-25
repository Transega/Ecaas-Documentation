########################
Data Processing & Access
########################

After Data is collected and submiited to the servers from the mobile application by the Enumerators,
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

i. Checking polygons if then fall withing farm boundaries.

ii. Editing polygons they may have inconsistenties with farm boundaries.

iii. Move the points that may have been collected but due to some reasons they have offsets to the farms 

iv. Check for duplicate polygons