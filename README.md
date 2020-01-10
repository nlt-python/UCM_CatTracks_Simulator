# UCM CatTracks Simulator
This work is licensed under the Creative Commons Attribution 4.0 International License.
To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ or
send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.  


## Project Status: *Active*


## Project Introduction/Objective
The purpose of this project is to simulate student wait times for the University of California at Merced's CatTracks bus system.

UC Merced, one of the newest University of California campuses in the San Joaquin Valley, began accepting undergraduate students in Fall 2005. Recently, their bus transit system, CatTracks, is experiencing a number of capacity issues. Students are expressing frustration about the wait and travel times to get to campus. A recurring issue is that the bus would fill up from all of the previous stops before arriving to campus. This project attempts to simulate the impact of scaling student load on bus stop wait times.


### Partner
* UC Merced
* https://www.ucmerced.edu/
* Partner contact: Michael Colvin


### Methods Used
* Data Cleaning
* Exploratory Data Analysis
* Data Visualization
* Predictive Modeling


### Technologies
* Bash scripting
* Python
* Pandas
* jupyter notebook
* matplotlib


## Project Description
(Provide more detailed overview of the project.  Talk a bit about your data sources and what questions and hypothesis you are exploring. What specific data analysis/visualization and modelling work are you using to solve the problem? What blockers and challenges are you facing?  Feel free to number or bullet point things here)

The data is primarily located in two xlxs workbooks containing ridership information from February 2019 and October 2018. Data from these months were selected since they are one of the few months during the school session in which buses run regularly and are not affected by holidays or the winter or summer breaks.

Each of these workbooks contain data on more than 12 bus lines on separate spreadsheets. As an early stage proof of concept, capacity and wait times will only be simulated for four bus lines. These lines were selected based on number of stops, weekday operation to cater to student need to take the bus to attend classes, and these lines being the ones students have expressed issues with. The main goal is to gain insight on which bus stops are most affected by upscaling ridership.

Some assumptions in the model:
- students do not exit the bus until they arrive on campus
- student wait times are averaged according to the number of students getting on the bus at a particular stop divided by the difference in time it takes for the previous and current bus to arrive at the desired stop.
- model used scheduled bus stop arrival times
  
  
## Project Approach

1. The data was imported into pandas and cleaned. Cleaning was required since the ridership spreadsheets contained:
   - inconsistent data such as variation in bus stop naming conventions between bus lines
   - mispelling of bus stop names
   - empty cells
   - cells with Nan data
   - random columns filled with "0"
   - random rows filled with "0"
   - time data of varying type
   - multi-indexed data
   - equivalent data between spreadsheets entered into incongruent cells
   
   ![Map of C2 Express Line (adapted from UC Merced)]https://github.com/nlt-python/UCM_CatTracks_Simulator/blob/master/Inked_c2_map.jpg

The bus stop on campus is at the Student Activities and Athletics Center (SAAC) and is the stop immediately after Arrow Wood Drive. Since the simulation is only interested in student wait times as they travel to campus, only data associated with bus stops headed toward campus is retained.

2. Bar graphs were made using matplotlib to explore ridership as a function of bus stop and time.

![October 2018 bus load data]https://github.com/nlt-python/UCM_CatTracks_Simulator/blob/master/Oct-2018-plot.png

Plot of the monthly total of students riding the bus at particular stops according to the bus lines C1-blue, C1-gold, C2-express and G-line. The stops listed on the x-axis going from left to right are headed toward campus. All stops listed after Muir Pass are leaving campus and thus not included in the graph.

![February 2019 bus load data]https://github.com/nlt-python/UCM_CatTracks_Simulator/blob/master/Oct-2018-time.png





- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting
- etc. (be as specific as possible)

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](Repo folder containing raw data) within this repo.

    *If using offline data mention that and how they may obtain the data from the froup)*
    
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...

*If your project is well underway and setup is fairly complicated (ie. requires installation of many packages) create another "setup.md" file and link to it here*  

5. Follow setup [instructions](Link to file)

## Featured Notebooks/Analysis/Deliverables
* [Notebook/Markdown/Slide Deck Title](link)
* [Notebook/Markdown/Slide DeckTitle](link)

