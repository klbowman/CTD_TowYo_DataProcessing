# CTD Tow-Yo Data Processing 

Python script to process Sea-Bird CTD data collected during a "Tow-Yo" operation.

## Description

This repository is designed to separate multiple "up" and "down" casts from an indivudal CTD data file. Tow-Yo is a technique used to search for anamolies in sensor data such as temperature, salinity, and beam attenuation (i.e., turbidity). This technique is used to search for plumes in the water column, such as those found at deep-sea hydrothermal vents. Sensor data is collected continuously as a CTD is towed from the back of a ship and repeatedly lowered up and down through the water column. 

SBE Data Processing software is designed to split one file into two separate data files - one "up" cast and one "down" cast file. Tow-Yo data files contain several series of increasing and decreasing depths, but SBE Data Processing Software will still only create two files, categorizing data as either up or down. The Python script shared here can be used to create indivudal files for any or all "up" and "down" casts of interest. 

The dashboard includes a drop-down menu that displays the numerical code for each individual sample. When a sample is selected, the “Demographic Info” panel is populated with metadata and the following three charts are populated with data:
* Bar graph displaying the top 10 OTUs by count
* Gauge plot showing the belly button scrubs per week
* Bubble plot displaying OTU counts for the entire sample

<p align="center">
  <img src="https://user-images.githubusercontent.com/74067302/145615550-98e49162-44c9-4e39-9050-ba837dc42863.png" alt="Dashboard Image"/>
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/74067302/145615561-5fc19f35-646b-47aa-9f63-4a93a495efe5.png" alt="Dashboard Image"/>
</p>

## Getting Started

### Technologies Used 

* JavaScript
* HTML
* CSS

### Installing

* Clone this repository to your desktop.
* Navigate to the home directory and open index.html in your browser.

### Data Sources

* Hulcr J, Latimer AM, Henley JB, Rountree NR, Fierer N, et al. (2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. PLoS ONE 7(11): e47712. doi:10.1371/journal.pone.0047712 [Access Data](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/)


## Author

Katlin Bowman, PhD

E: klbowman@ucsc.edu

[LinkedIn](https://www.linkedin.com/in/katlin-bowman/)
