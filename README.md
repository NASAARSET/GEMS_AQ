# GEMS_NASA
This repository contains:
1. Sample GEMS data file
2. Readme file
3. fileLists.txt file
4. Sample AERONET data file

There are four scripts: 

1) read_and_map_gems_no2_ai

a) Read the fileList and get the dataset/file(s) that is(are) listed.
b) Prompt the user to choose between "Y" and "N".
c) Calculate the range of valid data to be used to be displayed in the map.
d) Plot the variable of interest along with a color bar on the side based on the sds variable chosen and the data for that variable.

2) read_gems_and_list_sds

a) Read the fileList and get the dataset/file(s) that is(are) listed.
b) The main function calls another function to print the following values:
i) nc_attrs : list
  A Python list of the NetCDF file global attributes
ii) nc_dims : list
  A Python list of the NetCDF file dimensions
iii) nc_vars : list
  A Python list of the NetCDF file variables

3) read_gems_no2_ai_at_a_location

a) Read the fileList and get the dataset/file(s) that is(are) listed.
b) Calculate the mean, median, and standard deviation and display them.
c) Calculate the range of valid data and display the longitude and latitude.
d) User should input longitude and latitude that fall within the displayed range.
e) Identify points that are closest to the user input and output the value of the closest collocation, and the means of a 3x3 and 5x5 pixel square centered around the input.

4) read_gems_and_time_series_with_aeronet

a) Read the GEMS and AERONET file and get the dataset/file(s) that is(are) required (Aerosol Optical Depth).
b) Find GEMS pixel closest to AERONET Site.
d) Plot the variable of interest based on the sds variable (Aerosol Optical Depth) and the data for that variable.
