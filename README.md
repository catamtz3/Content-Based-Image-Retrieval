# Content-Based-Image-Retrieval

In this assignment, you will develop a content-based image retrieval system that retrieves database images based on their similarity with the query image.

The main idea is to represent each image (the database images and the query image) by a feature vector and then use a suitable distance measure to compute the distances between the query and database images and accordingly retrieve the images most similar to the query image.
In python, an image with height H, width W and number of channels C (3 for RGB images) is represented by a 3D matrix of shape H x W x C. To access a particular pixel (h,w) of a particular channel (c) of the 'image' variable, use image[h,w,c].
To compute the feature vector, you need to compute two histograms (see code to know how to do it):
Color histogram: You need to compute three types of color histogram
Convert the image into grayscale and compute a histogram with 8 bins (2 points)
Convert the image into grayscale and compute a histogram with 256 bins (2 points)
Compute an RGB histogram using the original image with the number of bins that performs better between the above two (3 points)
LBP (Local Binary Pattern) histogram: You need to compute two types of LBP histograms. Note that you need to first convert the RGB image into grayscale (given in the starter code)
Compute the histogram from the entire image. Ignore the boundary pixels. (3 points)
Divide the image into 16x16 regions, compute a 32-bin histogram for each region, and concatenate the histograms to get the final histogram. (3 points)
The default distance measure in the starter code is Euclidean distance. The code to compute the distances between image feature vectors, sort them and use them to retrieve images is already provided in the starter code. To use a different distance measure, change the distance name as input argument. Check the report to see which distance measures you need and what to do with different distance measures. The available names can be found here.
Fill in the tables, images and text in the report file. A sample output image is currently used as a placeholder.
Please write appropriate comments in your code.
