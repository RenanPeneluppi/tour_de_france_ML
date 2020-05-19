# tour_de_france_ML
This is a project to collect race data for Tour de france using web scrapping and with machine learning try to predict if a breakaway will be able to win a race.

### The break away in cycling – What makes a breakaway win possible
### By: Renan Peneluppi
#### A capstone project for BrainStation Data Science diploma program
### 1 – The Problem Statement
A break away in cycling is attempt for one rider, or a small group of riders, to gain distance from the main peloton in order to win a race. In many situations the break away is also a strategy to benefit a team member or to gain some tv broadcast time and make sponsors happy.
In the past the attributes that make a breakaway possible were always approached from the fitness and medical perspective, by measuring max Vo2 from athletes that perform well in these situations, or the power output decay over time from a rider on a small group compared to riders in big groups. As reliable as these are, they approach the training and fitness capacities of individual athletes, rather then race events that may be influenced by strategy.
The idea for this project came to me as I used to ride competitively and have always been a fan of the sport. To me some the most memorable stages in cycling are those where I got to cheer for the underdogs, or the one guy who managed to open a gap and by the end of the race gives everything to make it to the finish line while at every kilometers the gap is smaller and smaller.
From my knowledge and experience of the sport I aimed to prove that besides a few athletic characteristics a profile of a race and specific race events can also influence the outcome of a breakaway.
The goal of this data science approach is to evaluate race strategy based on race characteristics and rider profiles to determine what kind of race and race situation benefits a break away win.

### Please read the PDF file to get the main insights from this project. 

### 2 – Getting the data
Cycling is a sport currently collecting tons of data, however none of this data is collectively available, as professional riders will usually keep their most valuable data within the teams. In addition, most of the data available is to race results, and not specific in race events. To go around that the collected for this project is for all the Tour de France race stages from 1903 to 2019, except Time trial stages and canceled events.
In addition, every rider that won a stage but later had a result canceled due to doping was dropped from the final data set.
The technique used was web scraping with python pandas and beautiful soup packages, from the website https://www.procyclingstats.com/ for race results and riders information, looping thru every stage and every rider.
All scrapped tables and data were later combined into a full data set for analysis containing over 2600 unique rider details, almost 300 thousand rows and 16 features. This method was effective in combining scattered data, but also presented an expected challenge in data cleaning and normalization, where most definitely most time was spent.
