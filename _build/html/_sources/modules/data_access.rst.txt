########################
Data Processing & Access
########################

After Data is collected and submitted to the servers from the mobile application by the Enumerators.
A Data pipeline has already been set to establish the quality of data and flag out data that may be invalid.
This is done by some automated scripts dedicated to complete the process. Thereby, making it to be as efficient as possible as well as 
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

Given the importance this exercise the data collected by the Enumerators was subjuected to primary and secondary phases of data cleaning. 
The primary phase being the automated scripts while, the secondary phase; being the use of a Geospatial tool by a Geospatial Expert in 
data cleaning.

During this phase the following activities took place;

i. Ensuring the data has the correct map projection(s). 

ii. Checking polygons if then fall within farm boundaries.
    *This was done by visualizing the data on a GIS tool, and having satellite imagery as the basemap.*

iii. Editing polygons they may have inconsistenties with farm boundaries by looking at the base map.

iv. Moving the points that may have been collected but due to some reasons they have offsets to the farms.

v. Checking for duplicate polygons.

vi. Checking for overlapping polygons.


***************
Info about Data
***************

This section gives brief description of information about the data 

**Farm Polygon** - The farm polygon shows the coordinates of the boundary of the crop in the farm. When we do a Crop Cutting experiment, we place boxes where we will harvest our yield. When we are collecting the farm polygon we ensure that the polygon is for the crop in question and encapsulate the boxes we place. 
We have represented the polygons as WKT(Well Known Text) which is an ASCII representation of a spatial object with WGS84 projection.

**Case_ID** - This is a unique identifier for the data points that we have created. 

**Crop type** - We have different types of crops for the two countries which include; maize, groundnuts, Irish Potatoes, GreenGrams, Sorghum, Beans and Soya Beans.

**Planting & Harvesting Dates** - We have included these in order to understand about the crops’ lifecycle from when the crop was planted to when it was harvested. 

**Season** - In kenya we have two seasons, Short Rains and Long rains and in Zambia we only have one season, Main Season. 

**Crop Condition** - We collect the crop condition at the time of Box Placement. At this time, the crops are at their vegeatative state, and using observation techniques, one can easily determine their state. 

**Intercropping** - We collect data on intercropped fields, as most smallholder farmers prefer the aforementioned to maximize on the resources they have. If intercropped, we also name the crop that it has been intercropped with.

**Administrative Boundaries** - There are three levels of Admin Boundaries we were capturing, the Country being Level 0, upto to Adm Level 2.

**Final Weight and Yield** - We are collecting  weights of the crops from the boxes in (Kg) and changing them to yield per hectare depending on the size of the boxes which were majorly 8m by 5m boxes according to the Crop Cutting Protocols for the different crops that we used. 




***********
Data Access
***********

The datasets are archived by `PULA`_, they are free and can be downloaded on the following links;

**Vector file in CSV format** `here`_

.. _here: https://docs.google.com/spreadsheets/d/1IOOoFDlah5ahbTS6La5g544hHnCIV6c0ZlqdW1YS9uE/edit?usp=sharing

`PULA`_ is open and committed to further engagements on data collection, product development as well as offering insurance 
products to small holder farmers either through respective authories, farm co-perations and/or individual farmers.


.. _PULA: https://www.pula-advisors.com/



