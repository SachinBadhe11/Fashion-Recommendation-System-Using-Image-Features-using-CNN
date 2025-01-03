## Fashion-Recommendation-System-Using-Image-Features-using-CNN

This project demonstrates the implementation of a Fashion Recommendation System using image features extracted from a pre-trained convolutional neural network (CNN). The system recommends visually similar fashion items based on an input image.

## Project Overview
The Fashion Recommendation System:
- Utilizes a pre-trained VGG16 model to extract deep image features.
- Computes similarities between features to identify and recommend similar items.
- Visualizes the input and recommended images.

## Tools and Libraries
- **Google Colab**: For running the project.
- **Python Libraries**:
  - `tensorflow` and `keras` for deep learning.
  - `numpy` and `scipy` for numerical computations and similarity metrics.
  - `Pillow` and `matplotlib` for image processing and visualization.
  - `os` and `glob` for file and directory operations.
  - `zipfile` for handling compressed files.

## Dataset
The dataset is a collection of fashion item images stored in a zip file (`women-fashion.zip`). The zip file contains images organized under the directory `women-fashion/women fashion`.

## Features Implemented
1. **Dataset Extraction**: The zip file is extracted, and the images are listed for processing.
2. **Preprocessing**:
   - Images are resized to 224x224 pixels.
   - Images are normalized using `preprocess_input` from the VGG16 model.
3. **Feature Extraction**: Deep features are extracted using a pre-trained VGG16 model with the top layers removed.
4. **Similarity Calculation**:
   - Cosine similarity is used to compare features of the input image with all other images.
5. **Recommendations**:
   - The top-N similar images are displayed alongside the input image.

## How to Run the Project
### Step 1: Setup Google Colab
- Upload the `women-fashion.zip` file to the Colab runtime.
- Install necessary Python libraries if not already installed.

### Step 2: Execute the Code
Run the steps sequentially in Google Colab to extract the dataset, preprocess images, extract features, and generate recommendations.

## Output
- The input image is displayed alongside the top-N similar fashion items.

## Future Work
- Experiment with other pre-trained models such as ResNet or EfficientNet.
- Incorporate additional features like color or texture similarity.
- Build a web or mobile interface for users to upload images and receive recommendations.

## Acknowledgments
- **Dataset Source**: Provided as a zip file for demonstration.
- **Pre-trained Model**: VGG16 from Keras Applications.
