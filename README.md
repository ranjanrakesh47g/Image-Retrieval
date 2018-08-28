# Image-Retrieval

## Goal:
Given a query picture and an image database, retrieve images similar to the query image from the database.



## Data:
101_ObjectCategories dataset was used as the image database.

It consisted of around 10,000 images distributed among 101 categories.



## Model:
VGG16 model pretrained on ImageNet was used to obtain 4096-features of the images.



## Further steps:
The 4096-features were transformed into 300-length-vector using PCA.

Thereafter, distances were calculated between the query image and all other images in the database using the 300-length-vector represenatation of the images. And, images corresponding to least distances were returned.
