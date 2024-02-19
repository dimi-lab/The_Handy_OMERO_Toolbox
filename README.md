# The_Handy_OMERO_Toolbox
An assortment of scripts used to interface with our internal instance of OMERO and accomplish custom tasks

### How to use this repository?

*Each script is independant*

*Each jupyter notebook is single use*

*This is just a set of examples*

### Create a Config File for Authentication

Make a text file in "Documents" named "myKeyVariables.cfg" within which you place your authentication values

> [OMERO]
> pass = NNNNNNNN  
> user = username1
> url = omero.inst.edu

This file is how I can connect to my instance of OMERO without sharing my information. 


### Use Cases

1. Upload_Raw_MCD_To_Stiched_Scanplan.ipynb

	Open Hyperion MCD file, create a properly stitched scanplan image, then upload ROIs to represent the selection areas.
	
2. Labelled Mask To OMERO attempt.ipynb
	
	Read a labelled segmentation mask file, convert to polygon ROIs and upload to OMERO as layered segmentation annotation.