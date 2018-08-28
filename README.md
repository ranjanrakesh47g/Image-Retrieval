# Image-Retrieval

## Goal:
Given a query picture and an image database, retrieve images similar to the query image from the database.



## Data:
101_ObjectCategories dataset was used as the image database.

It consisted of around 10,000 images distributed among 101 categories.



## Model:
(1) VGG16 and (2) Resnet50 models pretrained on ImageNet were used to obtain representations of the images.


## Further steps:
The representations were transformed into 300-length-vector using PCA.

Thereafter, distances were calculated between the query image and all other images in the database using the 300-length-vector represenatation of the images. And, images corresponding to least distances were returned.
