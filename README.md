# CTD Tow-Yo Data Processing 

Python script to process Sea-Bird CTD data collected during a "Tow-Yo" operation.

## Description

This repository is designed to separate multiple "up" and "down" casts from an indivudal CTD data file. Tow-Yo is a technique used to search for anamolies in sensor data such as temperature, salinity, and beam attenuation (i.e., turbidity). This technique is used to search for plumes in the water column, such as those found at deep-sea hydrothermal vents. Sensor data is collected continuously as a CTD is towed from the back of a ship and repeatedly lowered up and down through the water column. 

SBE Data Processing software is designed to split one CTD data file into two separate files - one "up" cast and one "down" cast file. Tow-Yo data files contain several series of increasing and decreasing depths, however, SBE Data Processing Software can only categorize data as "up" or "down" and will still only create two files. The Python script shared here can be used to create indivudal files for any or all "up" and "down" casts of interest. This is accomplished by using time elapsed to bin data and isolate individual up and down casts.

The Jupyter Notebook file accomplishes the following steps:
* Removes rows of data tagged as bad (i.e., -9.990e-29 Bad_Flags values)
* Generates a plot of CTD depth verses time to visualize up and down casts
* Bin averages data on pressure
* Creates individual up and down cast files for any desired time interval

<p align="center">
  <img src="[https://user-images.githubusercontent.com/74067302/145615550-98e49162-44c9-4e39-9050-ba837dc42863.png](https://user-images.githubusercontent.com/74067302/232626692-7611c31a-140c-4e20-9ee6-b81e7a0eeabd.png)" alt="Plot of CTD depth verses time"/>
</p>

## Getting Started

### Technologies Used 

* Python
* Pandas
* Matplotlib

### Installing

* Clone this repository to your desktop.
* Navigate to the home directory and open Tow-Yo CTD Data Parsing.ipynb.
* Import unbinned SBE CTD data as a CSV file.

### Data Sources

* Hulcr J, Latimer AM, Henley JB, Rountree NR, Fierer N, et al. (2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. PLoS ONE 7(11): e47712. doi:10.1371/journal.pone.0047712 [Access Data](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/)


## Author

Katlin Bowman, PhD

E: klbowman@ucsc.edu

[LinkedIn](https://www.linkedin.com/in/katlin-bowman/)
