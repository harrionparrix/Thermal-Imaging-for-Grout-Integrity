# Imaging for Grout Integrity: Detecting and Quantifying Voids in Precast Structures using Computer Vision
This repository contains Python code snippets for various functions related to thermal imaging for grout integrity analysis. The functions provided here aid in detecting and quantifying voids in precast structures using computer vision techniques.

## Table of Contents
1. Dataset Generation
2. End to End Distance Estimation 
3. Centroid Distance Estimation 
4. Blob Length Estimation 
5. Blob Segmentation 
6. Volume Estimation: Spherical Approximation 
7. Volume Estimation: Maximum Dimension Approximation 
8. Volume Estimation: Largest Cross Sectional Dimension Approximation 
## Dataset Generation
The provided Python code generates a synthetic dataset for experimental purposes. It generates a 256x256 image with noise along with a corresponding mask.

## End to End Distance Estimation
This function computes the minimum distances between the end points of the convex hulls enclosing the detected blobs within an image. This metric aids in understanding the spatial distribution and separation between different blobs present in the image.

## Centroid Distance Estimation
This function calculates the distances between the centroids of detected blobs in the image. This measure provides insights into the distribution and spatial relationships between the centroids of different blobs, which can be crucial for various image analysis tasks.

## Blob Length Estimation
This function estimates the maximum lengths of the blobs detected in the image. By computing the maximum pairwise distances between the points on the contours of each blob, this function facilitates the characterization of blob shapes and sizes within the image.

## Blob Segmentation
This function performs blob segmentation on a binary image. It employs a connected components labeling algorithm to identify and segment individual blobs within the image.

## Volume Estimation: Spherical Approximation
This function takes an image as input and performs volume estimation using a spherical approximation method. It calculates the volume of each retained contour assuming spherical blob shapes.

## Volume Estimation: Maximum Dimension Approximation
This function conducts volume estimation using a maximum dimension approximation method. It calculates the area, volume, and maximum end-to-end distance for each retained contour.

## Volume Estimation: Largest Cross Sectional Dimension Approximation
This function conducts volume estimation using a largest cross-sectional dimension approximation method. It calculates the area and volume for each retained contour, where the volume is computed as the product of the area and the maximum dimension (width or height).
