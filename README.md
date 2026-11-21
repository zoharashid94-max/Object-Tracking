# Object Detection and Tracking Using OpenCV

## Project Overview

This project explores basic computer vision techniques for detecting and tracking objects across video frames. It was developed as part of my AI internship to gain practical experience with image processing, contour detection, and object tracking.

The implementation uses OpenCV to process video frames, apply image thresholding, detect contours, and track detected regions using their centroids. It also examines processing time and tracking behaviour during the experiment.

## Objectives

- Apply basic image processing techniques to video frames.
- Detect candidate objects using thresholding and contour analysis.
- Track detected regions using centroid-based matching.
- Measure processing time and approximate processing speed.
- Understand the limitations of classical computer vision tracking.

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- Jupyter Notebook

## Methodology

1. Load and process video frames.
2. Apply Gaussian blur to reduce image noise.
3. Use adaptive thresholding to create a binary image.
4. Detect external contours and filter them by area.
5. Calculate centroids for detected regions.
6. Associate detections across frames using centroid distance.
7. Evaluate processing speed and inspect tracking results.

## Experimental Setup

The recorded experiment used 100 frames at a resolution of 768 × 576 pixels, with a nominal frame rate of 25 FPS.

The implementation used contour-area filtering and centroid-distance matching to associate detections between frames. Tracking IDs were assigned by the implemented tracker.

## Results

In the recorded experiment:

- Mean valid contours detected per frame: 75.10
- Mean contour-processing time: 16.59 ms per frame
- Approximate contour-processing throughput: 60.81 FPS
- Mean tracking time: 23.22 ms per frame
- Approximate tracking throughput: 43.55 FPS
- Tracking IDs created during the run: 179

