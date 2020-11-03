# Data Visualization Project

The interactive tool displaying HIV patient information.

## Table of contents
* [Data](#data)
* [Questions](#questions)
* [Sketches](#sketches)
* [Visualizations](#visualizations)
* [Project Dashboard](#project-dashboard)
* [Project Video](#project-video)

## Data

The data I proposed to visualize for my project is the data from [Bangkok Smart Monotoring System](https://www.bkkbsms.com) which is the tool that keeps track of the HIV patient information. Its goal is to improve the quality of healthcare service and improve the HIV statistics in Bangkok overall. The data was processed into CSV provided in [Github Gist](https://gist.github.com/pichayutter/745d24ba99b6c30a4ba67b450ffe19c2). It contains the aggregated data of currently-on-treatment and new patient by quarter and district (out of 50 districts of Bangkok). 

<!--## Prototypes [P1] I’ve created a proof of concept visualization of this data. It's a Line Chart comparing the number of new cases of each district individually. It shows how many new HIV petient is in each quarter which can be easily compare and see the overall trend. The user can interact with the chart by select the districts from the DropDown menu at the top.![image](https://user-images.githubusercontent.com/70537588/95375088-23ec8680-08ad-11eb-998e-7412b5b80efd.png). [P2] I've integrated the Bangkok map using SVG & D3, which now can be interacted by MouseHover event. For the future work, I will integrate the dataset information into the created map template. So the map can show nice visualization of the data.![image](https://user-images.githubusercontent.com/70537588/95375639-e50b0080-08ad-11eb-85e4-8314bab6d8fd.png)-->

## Questions

The following questions drove the visualization and interaction decisions for this project:

 * How many new HIV cases compated across districts and how it changes over time?
 * Which district area of Bangkok has the most (and least) HIV density cases?
 * How the number of new HIV patient cases developed over time?

## Sketches

![image](https://user-images.githubusercontent.com/70537588/94599736-e3628c80-025e-11eb-9def-8e9549b95a41.png)
The idea behind this sketch is to analyze the trend of each district (1) alone and (2) their comparisons.

![image](https://user-images.githubusercontent.com/70537588/94599541-9088d500-025e-11eb-8d8d-16a562ed70b6.png)
The idea behind this sketch is to analyze the density of HIV patients around Bangkok and their trend over time.

## Visualizations

All visualization images are clickable which links to the [VizHub](vizhub.com) website for the real productions.

### New HIV Cases Line Chart by District

This visualization consists of line charts that shows the number of new HIV patients (in each district) throughout 2020. The visualization itself is interactive which allows selecting desired districts for comparisons to be analyzed.

Question being answered:
* How many new HIV cases compated across districts and how it changes over time?

For example, as shown in the picture below, the line charts show the information of district 21, 33, and 42. The most negative slope of district 21 tells us that even though, there are many new HIV cases in district 21 at the beginning of the year 2020, this number decreases dramatically.

[![image](https://user-images.githubusercontent.com/70537588/97954882-4ce23780-1dd7-11eb-9f4e-8d914f0cc549.png)](https://vizhub.com/pichayutter/88497edd1bcb466997c8d73dc10bf35d)

### Bangkok Map Aggregate Data

This visualization shows Bangkok map with the number of HIV patients. The circle size tells the number of cases (bigger circle means larger number and vice versa). The visualization itself is interactive which allows (1) switching between the number of currently-on-treatment and new patients, and (2) selecting which quarter of the year 2020 to represent the data.

Question being answered:
* Which district area of Bangkok has the most (and least) HIV density cases?
* How the number of new HIV patient cases developed over time?

For example, as shown in the picture below, the data presents overall trend of number of new HIV patients around Bangkok which district 10 seems to have the greatest number of new HIV patients. The map can also be used to analyze the density as well, which takes into account the district size. Although, district 10 has the highest number of cases due to its huge area, the circle shows on the map around that area is not that dense (compared to the green square region).

[![image](https://user-images.githubusercontent.com/70537588/97955833-bd8a5380-1dd9-11eb-938e-d54c3b4fc655.png)](https://vizhub.com/pichayutter/59557407084343e285357428b6f36885)

<!--## Schedule of Deliverables * Implement the interactive Bangkok map, including the ability to select multiple regions and the tooltip of each district number when mouse is hovered (To keep it simple without integrating the district name, I will keep the district number as main label. This will be changed to "Thai" district name later as an add-on after the project). Then, I will integrate the data into Bangkok map (S2). The circle size depends on the number of HIV patients on each district **by 14 October** * Add the interactive menu into the map (S2). This will allow the user to select which data to show in which quarter. **by 21 October** * [Deleted from plan: will focus on the interaction on two charts for final project] Implement S3 which combined all districts data together into the aggregated information each quarter as the Bar Chart. **by 28 October* * Add the interaction between selected region on maps to other chart (e.g. Line Chart, Bar Chart). **by 4 November**-->

## Project Dashboard

This dashboard consists of both visualizations which are linkable to each other. The map allows selecting the district region for comparison (instead of using its own dropdown menu). However since there is some data being shown in the map itself which causes come trouble when selecting the region. I intregated new toggle function which allows the user to toggle between (1) selection mode and (2) non-selection mode. The selection mode will hide all data in the map, so it is easily used for region selection. Key Shortcut for toggling between modes is pressing key 'S'.

[![ezgif com-gif-maker](https://user-images.githubusercontent.com/70537588/97956739-0d6a1a00-1ddc-11eb-8520-9169b89b468e.gif)](https://vizhub.com/pichayutter/704e01741dd74357a6e4a521cb562835)

## Project Video

TBD
