These are files from a research project by Caleb Griffy analyzing bicycle crashes in Chicago.
For more information on how this data was collected and how it was used, please read the attached paper.
For a brief overview on what each file in this repository was for:

1) Data was collected from these sources as of November 10th, 2024:
https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if/about_data
https://data.cityofchicago.org/Transportation/Traffic-Crashes-Vehicles/68nd-jvt3/about_data

These datasets contain crashes in Chicago and information about the vehicles involved.
Copies of this data is not contained in this GitHub, as they are kept more up to date on the Chicago site for free.
However, the following datasets created after data cleaning and splitting the files by type are provided.

2) The downloaded csv files were run through DataCleaning.ipynb.
This limited to crashes involving a bicycle, and split them into total, only fatal crashes, and only nonfatal crashes.
The files produced are stored in "Crashes by Type from Data Cleaning"

3) These files were used in the software QGIS in conjunction with the data from this source:
https://data.cityofchicago.org/Transportation/Bike-Routes/hvv9-38ut/about_data

Using these together, files were created to split the crashes on whether the crashes were within range of a bike route.
Spaces in each resulting csv represent an area of the city that's 200 meters by 200 meters.
In addition, a csv was made to represent which spaces in the grid are within Chicago's borders using this source:
https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-City/ewy2-6yfk

The results of this step are stored in "Crash Counts from QGIS"

4) The getEBEstimate.ipynb file was run with the different files, with the results being stored in "EB Estimate Results"

In addition, the getLocalDiff.ipynb and getCountMap.ipynb files were run.
The charts from the runs using all three of these notebook files are available in the paper, as well as discussion on them.

5) The file comparison.ipynb was just used to get some basic stats about the data.
These numbers were used in the paper, but were simple to obtain.



The paper can be found in the file "Caleb_Griffy_Geospatial_Analysis_of_Accidents_Involving_Bicycles_and_Bicycle_Route_Locations_in_Chicago.pdf"

I do plan to revisit this project for some of the changes and improvements brought up in the conclusion, and the GitHub will be updated to reflect that if so.