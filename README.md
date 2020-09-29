# Data Visualization Project

## Data

The data I propose to visualize for my project is the data from [Bangkok Smart Monotoring System](https://www.bkkbsms.com) which is the tool that keeps track of the HIV partient information. Its goal is to improve the quality of healthcare service and improve the HIV statistics in Bangkok overall. The data was processed into CSV provided in [Github Gist](https://gist.github.com/pichayutter/745d24ba99b6c30a4ba67b450ffe19c2). It contains the aggregated data of currently-on-treatment and new patient by quarter and district. 

## Prototypes

I’ve created a proof of concept visualization of this data. It's a Line Chart comparing the number of new cases of each district individually. It shows how many new HIV petient is in each quarter which can be easily compare and see the overall trend.
[![image](https://user-images.githubusercontent.com/70537588/94598604-30456380-025d-11eb-96e8-ad86ed6dcc7c.png)](https://vizhub.com/pichayutter/9f1b5422e90340729b1996ae37c65fda)

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * Q1 : The Line Chart (as shown in the prototype) will answer the question of comparing different district information. Also, we can see the correlation of the (total) number of HIV patients over time. Future task is to implement the interaction feature where the user can choose which district to display in the Line Chart.
 * Q2 : What is the density of the overall HIV patient around Bangkok? The plan is to intregate the data to the Bangkok map in order to visualize the data using the size and color.
 * Q3 : How overall number of patients change by quater? The plan is to build the bar chart aggregated by each quarter that tells the number of currently-on-treatment and new patients.

## Sketches

![image](https://user-images.githubusercontent.com/70537588/94599736-e3628c80-025e-11eb-9def-8e9549b95a41.png)
Q1 : This answer Q1 which allows the interaction between user to select the districts need to be compared. It is useful to compare 2-3 districts at the time to see the trend. It can also be used to look at 1 district alone to see the improvement of the treatment as well (less cases over time can imply better quality).

![image](https://user-images.githubusercontent.com/70537588/94599541-9088d500-025e-11eb-8d8d-16a562ed70b6.png)
Q2 : This sketch answer Q2 which we can see the density (and also the circle size) to see trend of where HIV patient lives around Bangkok. This can improve the quality of cure spefically to that district.

![image](https://user-images.githubusercontent.com/70537588/94599963-3a686180-025f-11eb-836e-cdd564c6ed77.png)
Q3 : This answers the Q3 where we aggregate just by quarter so total number of HIV patients in Bangkok can be analyzed.

## Open Questions

I'm still researching how to intregate the Bangkok map to the visualization since I only see the SVG of Bangkok map but some visualization tool allows only GeoJSON file. I have seen [the tutorial of how to integrate the SVG map into D3](http://bl.ocks.org/catherinekerr/e345a906f8e2bae8d07dbc79f8f04036), but haven't tried yet.
