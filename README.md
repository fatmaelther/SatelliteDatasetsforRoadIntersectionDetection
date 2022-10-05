# Using-Satellite-Images-Datasets-for-Road-Intersection-Detection-in-Route-Planning
Dataset Automatic Acquisition and Annotation

Understanding road networks plays an important role in navigation applications such as self-driving
vehicles and route planning for individual journeys. Intersections of roads are essential components
of road networks. Understanding the features of an intersection, from a simple T-junction to larger
multi-road junctions is critical to decisions such as crossing roads or selecting safest routes. The
identification and profiling of intersections from satellite images is a challenging task. While deep
learning approaches offer state-of-the-art in image classification and detection, the availability of
training datasets is a bottleneck in this approach. A novel labelled satellite image dataset for the
intersection recognition problem is presented. consisting of 14,692 satellite images of Washington
DC, USA. To support other users of the dataset, an automated download and labelling script is
provided for dataset replication.

A constant problem in our work is lack of shared datasets. It is desirable to make the two datasets
constructed here available to the research community. The terms of Google API prevent the direct
publishing or distribution to others. In order for others researchers to access the dataset, we have
provided an automated script to generate replica datasets via the Google maps static API, but using
the API key of the downloader. The script will automatically download the exact same images for
either/both satellite and hybrid – and apply the correct annotation of our dataset. The images used
in these datasets were downloaded without cost, using the free allocation of images for Google
maps static API, as at publication date.
After capturing and annotating the dataset, two types of datasets were constructed: a satellite
intersection dataset and a hybrid intersection dataset. Each one has two classes: intersection and

no-intersection. In each dataset, the intersection category contains 7342 images and the no-
intersection category contains 7350 images.

This folder contains the annotation folder for our dataset and a script file:
1. The annotation folder contains four files. Two of them are annotation files for testing
images: one for intersection class and another one for no_intersection class. Other two of
them are annotation files for training and validation images: one for intersection class and
another one for no_intersection class.
2. The script file is a python script to download images form google using maps static API and
create dataset folder. After running this code, a dataset folder will be created.

To run this script, you need to enter the following parameters: api_key, maptype,
annottation_folder_path, and destination_path.
1. api_key: To download images form Google map, you need to create a project with a billing
account. Then, you must enable the maps static API. Then, use this API key in our script. For
more details about how to create this API, follow instructions in this link.
https://developers.google.com/maps/documentation/maps-static/get-api-key
2. maptype: you have to identify which type of image do you want to include in dataset. We
used two type satellite or hybrid. Before you run the script, be sure that you use the one you
want.
3. annottation_folder_path: In this field, put the path for the annotation folder that associated
with this script.
4. destination_path: In this filed, define a path to a create dataset folder in it.


Recommended Citation:
@article{ title     = {Using Satellite Images Datasets for Road Intersection Detection in Route Planning},
	  author    = {Fatma El-zahraa El-taher and  Ayman Taha and  Jane Courtney and  Susan Mckeever},
	  country	= {},
	  institution	= {},
	    journal   = {International Journal of Computer and Systems Engineering},
	  volume    = {16},
	  number    = {10},
	  year      = {2022},
	  pages     = {411 - 418},
	  ee        = {https://publications.waset.org/pdf/10012708},
	  url   	= {https://publications.waset.org/vol/190},
	  bibsource = {https://publications.waset.org/},
	  issn  	= {eISSN: 1307-6892},
	  publisher = {World Academy of Science, Engineering and Technology},
	  index 	= {Open Science Index 190, 2022},
	}
