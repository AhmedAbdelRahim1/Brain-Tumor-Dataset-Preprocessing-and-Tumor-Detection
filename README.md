# Brain Tumor Image Dataset Preprocessing

# Introduction & Data Format
This repository provides a comprehensive guide on preprocessing a dataset containing grayscale images of infected patients' brain X-rays. The preprocessing steps outlined below are essential to ensure the dataset is clean, well-organized, and ready for use in machine-learning tasks related to brain tumor detection.

- Data Type: Grayscale images <br />
- Number of Images: 10 <br />
- Image Dimensions: 256x256 <br />

# Preprocessing Steps

Data Cleaning:

- Handling any corrupted or unreadable images by only reading the valid images.
- Ensuring that all images have consistent dimensions by resizing them to 256x256.

Data Transformation:

- Image Augmentation : 
Applying data augmentation techniques such as rotation, flipping, and cropping to 4 equal parts to increase the image data's diversity.
- Normalize Pixel Values: Scale pixel values to a specific range (e.g., [0, 1] or [-1, 1]) to ensure uniformity in data distribution. This step is crucial for model convergence.
- Convert Images to NumPy Arrays: Convert the image data into NumPy arrays for compatibility with machine learning frameworks.

# Data Splitting

- Splitting the dataset into training, validation, and test sets. A typical split ratio is 70-80% for training, 10-15% for validation, and 10-15% for testing. Ensure that the data distribution among classes is balanced in each split.

Data Storage:

- All the preprocessed images and their corresponding labels are saved in a .CSV file.


