# Vehicle Detection and Tracking using SVM

This project focuses on implementing vehicle detection and tracking using a Support Vector Machine (SVM) classifier. The pipeline includes various stages such as extracting features from images, training the SVM classifier.

## Project Structure

The project directory is organized as follows:

- **data:** Contains image data for both vehicles and non-vehicles.
  - **vehicles:** Subdirectory containing images of vehicles.
  - **non-vehicles:** Subdirectory containing images of non-vehicles.

- **code:**
  - **vehicle_detection.ipynb:** Jupyter Notebook containing the main code for the vehicle detection and tracking pipeline.

## Features
1. Bounding Box Drawing
The project includes a function draw_boxes that takes an image and a list of bounding boxes as inputs, then draws the boxes on the image using OpenCV.

2. Template Matching
Template matching is implemented to locate objects in an image using a template. The find_matches function identifies matches and draws bounding boxes around them.

3. Color Histograms
Color histograms are computed to extract color features from images. The color_hist function generates histograms for the RGB channels.

4. Histogram of Oriented Gradients (HOG)
The HOG features are extracted from images using the get_hog_features function. It includes a visualization of the HOG features for better understanding.

5. Data Exploration
The project explores the data by providing information about the number of car and non-car images, image shape, and data type.

6. Feature Extraction
Features are extracted from images using functions like bin_spatial and color_hist. The extracted features are then used to train the SVM classifier.

7. SVM Classifier
A Linear SVM classifier is trained on the extracted features to distinguish between car and non-car images. The classifier achieves a high accuracy on the test dataset.
