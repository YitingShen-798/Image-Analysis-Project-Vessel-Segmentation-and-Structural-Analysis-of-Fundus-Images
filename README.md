# Image-Analysis-Project-Vessel-Segmentation-and-Structural-Analysis-of-Fundus-Images

## Overview
This project focuses on the extraction, segmentation, and morphological analysis of retinal blood vessels from fundus images.
The dataset consists of high-resolution fundus images and manual binary segmentation masks, sourced from https://www5.cs.fau.de/research/data/fundus-images/.

## Project Structure
### Part 1: Vessel Segmentation
Step 1: Load the color fundus image and display each color channel (Red, Green, Blue).

Step 2: Convert the image to HSV color space and display the Hue, Saturation, and Value channels.

Step 3: Segment vessels by applying:
Adaptive Histogram Equalization
Local thresholding
Morphological operations

Step 4: Overlay the segmentation results with the provided manual annotation mask to visualize agreement and disagreement.

Step 5: Calculate the Dice coefficient and/or Jaccard index to quantify segmentation accuracy.

### Part 2: Vascular Network Analysis

Step 1: Remove small vessels (less than 8 pixels wide) using morphological opening.

Step 2: Apply morphological thinning to extract a 1-pixel wide vascular skeleton.

Step 3: Count the number of pixels in the skeleton to measure the total vascular length.

Step 4: Identify and measure vascular structures wider than 20 pixels.

Step 5: Compute the orientation distribution of the thinned vessels and visualize it in a polar (rose) plot.

## Requirements

Main packages used: numpy, scikit-image, matplotlib, scikit-learn


