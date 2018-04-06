# Night-Knights-dataset

Night Knight is a GWAP that aims to classify images taken from the International Space Station (ISS) into a set predefined categories.

The six possible categories are mapped in the following codes:
* 1 = black
* 2 = city
* 3 = stars
* 4 = aurora
* 5 = iss 
* 6 = none

Below we describe the structure of the datasets stored in this repository, detailing the meaning of all the columns of the .csv files. 

## Dataset1
File with the log of the users' classifications. 

Columns description: 
* _idResource_: ID of the image classified
* _idUser_: ID of the user
* _chosenCategory_: class selected by the user
* _incentive_: with possible values "EXTRINSIC" and "INTRINSIC", indicats the type of incentive available when the image has been played. "EXTRINSIC" indicate a period with a tangible reward (i.e. during a competition), "INTRINSIC" indicate an intangible reward like fun.  


## Dataset2
List of all the images classified with the final classification assigned after having run the aggregation algorithm on all the users' contributions. 

Columns description:
* _idResource_: ID of the image classified
* _aggregateCategory_: final classification

## Dataset3
List of all the images played in the game with the URL to the NASA website. 

Columns description:
* _idResource_: ID of the image classified
* _refUrl_: url of the NASA page with the image
