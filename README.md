# int-247-km007-ca-2-santosh199518
A project on Image Classification where we can classify the image into different classes based upon data given in it.

It consists on three files:
- Segmentation_train.csv: The file containing the training data for classification.
- Segmentation_test.csv:  The File containing the testting data for classification.
- Segmentation.names:     The file contating names of attributes present in the data.
These data has been taken from UCI Machine Learning Repository.

# Image Segmentation:
# Introduction
In digital image processing and computer vision, image segmentation is the process of partitioning a digital image into multiple segments (sets of pixels, also known as image objects). The goal of segmentation is to simplify and/or change the representation of an image into something that is more meaningful and easier to analyze. Image segmentation is typically used to locate objects and boundaries (lines, curves, etc.) in images. More precisely, image segmentation is the process of assigning a label to every pixel in an image such that pixels with the same label share certain characteristics.

The result of image segmentation is a set of segments that collectively cover the entire image, or a set of contours extracted from the image (see edge detection). Each of the pixels in a region are similar with respect to some characteristic or computed property, such as color, intensity, or texture.

# Some information about data
# Attribute Description:
-  region-centroid-col:  the column of the center pixel of the region.
- region-centroid-row:  the row of the center pixel of the region.
- region-pixel-count:  the number of pixels in a region = 9.
- short-line-density-5:  the results of a line extractoin algorithm that counts how many lines of length 5 (any orientation) with low contrast, less than or equal to 5, go through the region.
- short-line-density-2:  same as short-line-density-5 but counts lines
         of high contrast, greater than 5.
- vedge-mean:  measure the contrast of horizontally adjacent pixels in the region.  There are 6, the mean and standard deviation are given.  This attribute is used as a vertical edge detector.
- vegde-sd:  (see 6)
- hedge-mean:  measures the contrast of vertically adjacent pixels. Used for horizontal line detection. 
- hedge-sd: (see 8).
- intensity-mean:  the average over the region of (R + G + B)/3
- rawred-mean: the average over the region of the R value.
- rawblue-mean: the average over the region of the B value.
- rawgreen-mean: the average over the region of the G value.
- exred-mean: measure the excess red:  (2R - (G + B))
- exblue-mean: measure the excess blue:  (2B - (G + R))
- exgreen-mean: measure the excess green:  (2G - (R + B))
- value-mean:  3-d nonlinear transformation of RGB. (Algorithm can be found in Foley and VanDam, Fundamentals of Interactive Computer Graphics)
- saturation-mean:  (see 17)
- hue-mean:  (see 17)
These are the real time attributes obtained from an image after segmentation. Now we need to classify the given images into different target classes which are:
# Classes:  brickface, sky, foliage, cement, window, path, grass.
# Number of Attributes: 19 continuous attributes
# Number of Instances: Training data: 210  Test data: 2100
# Missing Attribute Values: None
