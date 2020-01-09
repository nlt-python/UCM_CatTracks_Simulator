# UCM_CatTracks_Simulator

Python simulation of student wait times for the University of California at Merced's CatTracks bus system

UC Merced, one of the newest University of California campuses, began accepting undergraduate students in Fall 2005. Recently, their bus transit system, CatTracks, is experiencing a number of capacity issues. Students are complaining about the wait and travel times to get to campus. A recurring issue is that the bus would fill up from all of the previous stops before arriving to campus.

I am building a model to simulate student wait times at the various bus stops offered by UCM's CatTracks system using a combination of Python programming, pandas, matplotlib and bash scripting. Data is primarily located in two spreadsheets containing ridership information from February 2019 and October 2018. Data from February 2019 and October 2018 were selected since they are one of the few months during the school session not affected by holidays. 

Each of these spreadsheets contain data on more than 12 bus lines on separate worksheets, but for the purposes of this project, capacity and wait times will only be simulated for three bus lines. These lines were selected based on number of stops, weekday operation to cater to student need to take the bus to attend classes, and these bus lines being the ones students have expressed issues about.

