# The_Handy_OMERO_Toolbox
An assortment of scripts used to interface with our internal instance of OMERO and accomplish custom tasks

## How to use this repository?

*Each script is independant*

*Each jupyter notebook is single use*

*This is just a set of examples, of things I needed for a project*

## Create a Config File for Authentication

Make a text file in "Documents" named "myKeyVariables.cfg" within which you place your authentication values

> [OMERO]
>
> pass = NNNNNNNN  
>
> user = username1
>
> url = omero.inst.edu
>

This file is how I can connect to my instance of OMERO without sharing my information. 


## Use Cases

1. `Upload_Raw_MCD_To_Stiched_Scanplan.ipynb`

	Open Hyperion MCD file, create a properly stitched scanplan image, then upload ROIs to represent the selection areas.
	
2. `Labelled Mask To OMERO attempt.ipynb`
	
	Read a labelled segmentation mask file, convert to polygon ROIs and upload to OMERO as layered segmentation annotation.
	
3. `Upload meta datatable for single TMA project.ipynb`

	Read data table, filled with lots of information about the origin of each image, structure and submit to OMERO for explorable and searchable annotation
	
4. `Upload meta datatable for single TMA project part 2.ipynb`

	Read data table, previous excel file, identifying single image quality, sort and submit to OMERO, as if it was originally noted there.

5. `Retrieve Points of Annotation from Whole Project.ipynb`

	Loop every dataset, every image in a single project, and record out each image's point annotations, formatted for QuPath points importing. Also will genreate a summary log file, with quick counts on annotation labels.
