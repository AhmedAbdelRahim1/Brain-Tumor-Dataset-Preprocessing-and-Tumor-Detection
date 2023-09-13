# Brain Tumor Image Dataset Preprocessing

# Introduction & Data Format
This repository provides a comprehensive guide on preprocessing a dataset containing grayscale images of infected patients' brain X-rays. The preprocessing steps outlined below are essential to ensure the dataset is clean, well-organized, and ready for use in machine-learning tasks related to brain tumor detection.

Data Format: <br />
- Data Type: Grayscale images <br />
- Number of Images: 10 <br />
- Image Dimensions: 256x256 <br />

# Preprocessing & Storing Steps

Data Cleaning:

- Handling any corrupted or unreadable images by only reading the valid images.
- Ensuring that all images have consistent dimensions by resizing them to 256x256.

Data Transformation:

- Image Augmentation: Applying data augmentation techniques such as rotation, flipping, and cropping to 4 equal parts to each image.
- Converting Images to NumPy Arrays: Convert the image data into NumPy arrays for compatibility with machine learning frameworks.

Data Storage:

- All the preprocessed images are saved in NumPy Arrays to be compatible with the machine learning frameworks.


