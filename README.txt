README for vis_calc_general.ipynb
Version: 1.0 11/15/2019
Author(s): Wataru Hayashi, Derek Moore, Trevor Stanfill

Interactive notebook python script for use with Jupyter Notebook
Written in Python 2
Purpose: Visibility Calculator for the Great Basin Observatory (GBO)
-	Outputs azimuth, altitude, and airmass for an object with respect to GBO at midnight for a user-input date.
-	Plots azimuth and airmass of the object over the course of the night.

Based on astropy documentation: "Determining and plotting the altitude/azimuth of a celestial object"
https://docs.astropy.org/en/stable/generated/examples/coordinates/plot_obs-planning.html

USING THE VISIBILITY CALCULATOR
The user-input parameters are ONLY in the first code cell, there is no need to change any variables after the first code cell.
There are two parameters: the source (object to be observed), and the date of observation.
-	For the source, there are two ways to input the paramter:
	-	Set the sourceName variable to the source's name (check the name with the SIMBAD database) and set sourceIndex = 0
			OR
	-	Set the rightAsc and declination variables to the ICRS coordinates of the source and set sourceIndex = 1
-	For the date (obsTime variable), it should follow this format: 'yyyy-mm-dd 00:00:00'
	-	Keep in mind that midnight is the following day
		-	e.g. if the night of observation is October 5th, 2019, then obsTime = '2019-10-06 00:00:00'

