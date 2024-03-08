# Eye Diseases Classification Project with XAI techniques

This project aims to classify images of eyes into different categories of diseases using deep learning models. The dataset used for this project is publicly available on Kaggle https://www.kaggle.com/datasets/gunavenkatdoddi/eye-diseases-classification?select=dataset

## Dataset Analysis

The `dataset_analysis` function in the code analyzes the dataset by inspecting the image files in each category folder. It provides information about the number of images, their formats, and dimensions.

## CSV File Creation

The script creates a CSV file containing the image paths and corresponding labels extracted from the dataset folders.

## Dataset Splitting

The dataset is split into training, validation, and test sets using the `train_test_split` function from scikit-learn. The split datasets are saved into separate CSV files.

## Image Preprocessing

Images in the datasets are preprocessed by resizing them to a standard size (224x224) and normalizing their pixel values.

## Model Training

Two deep learning models, VGG16 and MobileNet, are trained on the preprocessed images. The training loop involves iterating over epochs and batches, computing gradients, and updating model parameters.

## Model Evaluation

The trained models are evaluated on the test set to measure their accuracy in classifying eye disease images.

## Visualization

Integrated gradients are computed to generate attribution heatmaps, highlighting regions of importance in input images for better interpretability.

## Results

Validation accuracy and loss curves are plotted for comparison between VGG16 and MobileNet models.

## GitHub Description

This repository contains code for an eye diseases classification project using deep learning models. It includes dataset analysis, preprocessing, model training, evaluation, and visualization. Two popular models, VGG16 and MobileNet, are trained and compared for accuracy in classifying images of different eye diseases.

## Explainable AI (XAI) Techniques

This project incorporates Explainable AI (XAI) techniques to provide insights into model predictions and enhance interpretability. Here's how XAI techniques are utilized in this project:

### Integrated Gradients

Integrated gradients are computed to generate attribution heatmaps, highlighting regions of importance in input images. By visualizing these heatmaps, users can understand which parts of the image are contributing the most to the model's decision-making process. This enhances interpretability and provides insights into why the model made a particular prediction.

### Visualization

The generated attribution heatmaps are visualized alongside the original input images. This visualization allows users to directly observe the areas of the image that the model focuses on when making predictions. By comparing the original image with the heatmap, users can gain insights into how the model interprets features relevant to classifying eye diseases.

### Usage

To utilize XAI techniques in this project:

1. Run the provided scripts to train the VGG16 and MobileNet models on the eye diseases dataset.
2. After training, use the `visualize_attributions` function to generate attribution heatmaps for specific images.
3. Visualize the original images alongside the generated heatmaps to understand the model's decision-making process.

By incorporating XAI techniques, this project aims to enhance transparency, trust, and understanding of deep learning models used for eye disease classification.

Feel free to explore the provided code and experiment with different images to gain deeper insights into the model's behavior!
