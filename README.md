# Advanced Lane Finding
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

### Summary

Steps of this project were the following:  

1. Do Camera Calibration
2. Implement Still Image Pipeline. As a result, the original image has an overlay marking 
lane boundaries, and numererical estimations of the curvature and vehicle position.
  1. Apply the distortion correction to the raw image.  
  2. Apply a perspective transform to rectify binary image ("birds-eye view"). 
  3. Use color transforms, gradients, etc., to create a thresholded binary image.
  4. Detect lane pixels and fit to find lane boundary.
  5. Determine curvature of the lane and vehicle position with respect to center.
  6. Warp the detected lane boundaries back onto the original image.
3. Implement Video Pipeline. As a result, 

## 1. Camera Calibration

**GOAL:** *Compute the camera calibration matrix and distortion coefficients
given a set of chessboard images.*

<img src="./output_images/calibration.png" alt="Calibration result" width="800">

## 2. Still Image Pipeline Implementation

**GOAL:** *Output visual display of the lane boundaries and numerical estimation of lane 
curvature and vehicle position.*

### 2.1 Distortion Correction

**GOAL:** *Apply the distortion correction to the raw image.*

<img src="./output_images/correct_distortion.png" alt="Corrected distortion" width="800">

### 2.2 Perspective Transform

**GOAL:** *Apply a perspective transform to rectify the image ("birds-eye view")*

### 2.3 Lane Line Masking

**GOAL:** *Use color transforms, gradients, etc., to create a thresholded binary image.*

<img src="./output_images/mask.png" alt="Thresholded bitmask with lane line" width="800">

### 2.4 Lane Line Finding

**GOAL:** *Detect lane pixels and fit to find lane boundary.*

<img src="./output_images/histogram.png" alt="Initials line positions" width="600">
<img src="./output_images/line_finding.png" alt="Sliding windows" width="800">
<img src="./output_images/polyfit.png" alt="Fitted polynomial" width="800">


### 2.5 Lane Curvature and Car Position Calculation

**GOAL:** *Determine curvature of the lane and vehicle position with respect to center.*

### 2.6 Lane Overlay Generation
 
**GOAL:** *Output visual display of the lane boundaries*

<img src="./output_images/test_images_with_lane_overlays.png" alt="Images with lane overlays" width="800">

## 3. Video Pipeline Implementation
## 4. Discussion

