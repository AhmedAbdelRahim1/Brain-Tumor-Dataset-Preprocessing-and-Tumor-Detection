# Brain Tumor Image Dataset Preprocessing

# Introduction & Data Format
This repository provides a comprehensive guide on preprocessing a dataset containing grayscale images of infected patients' brain X-rays. The preprocessing steps outlined below are essential to ensure the dataset is clean, well-organized, and ready for use in machine-learning tasks related to brain tumor detection.

Data Format: <br />
- Data Type: Grayscale images <br />
- Number of Images: 10 <br />
- Image Dimensions: 256x256 <br />

# Preprocessing & Storing Methodoloies

Data Cleaning:

- Handling any corrupted or unreadable images by only reading the valid images.
- Ensuring that all images have consistent dimensions by resizing them to 256x256.

Data Transformation:

- Image Augmentation: Applying data augmentation techniques such as rotation, flipping, and cropping to 4 equal parts to each image.
- Converting Images to NumPy Arrays: Convert the image data into NumPy arrays for compatibility with machine learning frameworks.

Data Storage:

- All the preprocessed images are saved in NumPy Arrays to be compatible with the machine learning frameworks.

# Tumor Detection

The Tumor Detection part focuses on the precise identification and segmentation of brain tumors within medical images. This critical medical imaging task is achieved through a multi-step process, leveraging state-of-the-art computer vision techniques and the OpenCV library.

# Tumor Detection Methodology
- Color Range Extraction: The initial step involves the extraction of color ranges corresponding to brain tumors within each medical image. This step forms the foundation for subsequent tumor segmentation.

- Segmentation with OpenCV: The OpenCV library plays a pivotal role in segmenting the tumors from the images. The .inRange() function is utilized for this purpose, allowing for the isolation of the tumor regions.

- Tumor Cropping: Following successful segmentation, individual tumors are cropped from their respective images using image-slicing techniques. This step facilitates the isolation of the tumor regions, which are essential for subsequent analysis.

- Refined Tumor Segmentation: To enhance model accuracy and precision, a specialized algorithm is implemented. This algorithm further refines the tumor segmentation process, ensuring that only the tumor itself is included in the segmented region, without any extraneous pixels. This meticulous refinement is crucial for the reliable detection of brain tumors.
