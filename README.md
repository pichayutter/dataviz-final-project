# Data Visualization Project

## Data

The data I propose to visualize for my project is the data from [Bangkok Smart Monotoring System](https://www.bkkbsms.com) which is the tool that keeps track of the HIV partient information. Its goal is to improve the quality of healthcare service and improve the HIV statistics in Bangkok overall. The data was processed into CSV provided in [Github Gist](https://gist.github.com/pichayutter/745d24ba99b6c30a4ba67b450ffe19c2). It contains the aggregated data of currently-on-treatment and new patient by quarter and district. 

## Prototypes

[P1] I’ve created a proof of concept visualization of this data. It's a Line Chart comparing the number of new cases of each district individually. It shows how many new HIV petient is in each quarter which can be easily compare and see the overall trend. The user can interact with the chart by select the districts from the DropDown menu at the top.
![image](https://user-images.githubusercontent.com/70537588/95375088-23ec8680-08ad-11eb-998e-7412b5b80efd.png).

[P2] I've integrated the Bangkok map using SVG & D3, which now can be interacted by MouseHover event. For the future work, I will integrate the dataset information into the created map template. So the map can show nice visualization of the data.
![image](https://user-images.githubusercontent.com/70537588/95375639-e50b0080-08ad-11eb-85e4-8314bab6d8fd.png)

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * Q1 : The Line Chart (as shown in the prototype) will answer the question of comparing different district information. Also, we can see the correlation of the (total) number of HIV patients over time (see Prototype [P1])
   * Future implementation is (instead of select the districts from the Dropdown menu), use can click the region of each district from the map (Q2) which will also change this Line Chart.
 * Q2 : What is the density of the overall HIV patient around Bangkok? The plan is to intregate the data to the Bangkok map in order to visualize the data using the size and color.
   * Template is done (see Prototype [P2])
 * Q3 : How overall number of patients change by quater? The plan is to build the bar chart aggregated by each quarter that tells the number of currently-on-treatment and new patients.

## Sketches

![image](https://user-images.githubusercontent.com/70537588/94599736-e3628c80-025e-11eb-9def-8e9549b95a41.png)
S1 : This answer Q1 which allows the interaction between user to select the districts need to be compared. It is useful to compare 2-3 districts at the time to see the trend. It can also be used to look at 1 district alone to see the improvement of the treatment as well (less cases over time can imply better quality).

![image](https://user-images.githubusercontent.com/70537588/94599541-9088d500-025e-11eb-8d8d-16a562ed70b6.png)
S2 : This sketch answer Q2 which we can see the density (and also the circle size) to see trend of where HIV patient lives around Bangkok. This can improve the quality of cure spefically to that district.

## Schedule of Deliverables

 * Implement the interactive Bangkok map, including the ability to select multiple regions and the tooltip of each district number when mouse is hovered (To keep it simple without integrating the district name, I will keep the district number as main label. This will be changed to "Thai" district name later as an add-on after the project). Then, I will integrate the data into Bangkok map (S2). The circle size depends on the number of HIV patients on each district **by 14 October**
 
 * Add the interactive menu into the map (S2). This will allow the user to select which data to show in which quarter. **by 21 October**
 
 * [Deleted from plan: will focus on the interaction on two charts for final project] Implement S3 which combined all districts data together into the aggregated information each quarter as the Bar Chart. **by 28 October**
 
 * Add the interaction between selected region on maps to other chart (e.g. Line Chart, Bar Chart). **by 4 November**
