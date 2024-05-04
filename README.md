# Crop Classifier Using KMeans

This repository provides a classification solution for hyperspectral images (HSI) using KMeans clustering. The solution primarily focuses on classifying different crop types based on their spectral signatures.

## Key Features

- **Hyperspectral Image Classification**: This solution processes hyperspectral images and categorizes them based on their spectral properties.
- **KMeans Clustering**: The main clustering technique used is KMeans, which effectively identifies and groups similar spectral data points.
- **Dataframe Manipulation**: The class transforms the image and ground truth into a Pandas DataFrame for easy manipulation and processing.
- **Data Normalization**: The class includes a normalization method to scale the data appropriately for clustering.
- **Visualizations**: The solution includes various visualization methods to display hyperspectral bands, crop labels, and classification maps.
- **Random Pixel Selection**: The class can randomly select pixels to display their spectral signatures, which helps in understanding the crop type distribution.

## Dependencies

- **Python 3.7+**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Scikit-learn**

## Class Structure

The `HSI_Classification` class is designed to handle hyperspectral images. Below is an overview of the key methods:

- **Initialization (`__init__`)**: Sets up the initial properties including the image, ground truth, labels, and dimensions. Also prepares the data as a Pandas DataFrame.
- **DataFrame Setup (`df_setup`)**: Reshapes the image and ground truth and combines them into a DataFrame.
- **DataFrame Cleaning (`df_clean`)**: Removes unwanted labels from the DataFrame.
- **Extract Features and Labels (`extract_X_y`)**: Separates the features and labels from the DataFrame.
- **Draw Bands (`draw_bands`)**: Displays specific bands of the hyperspectral image.
- **Draw Labels (`draw_labels`)**: Visualizes the ground truth labels.
- **Draw Classification Map (`draw_clmap`)**: Visualizes the classification map using a provided prediction.
- **Get Random Pixels (`get_random_pixels`)**: Returns a list of randomly selected pixels for each category.
- **Plot Pixel Signature (`plot_pixel_signature`)**: Plots the spectral signature of randomly selected pixels.
- **Normalize (`normalize`)**: Normalizes the data using a MinMaxScaler.
- **Choose Centroids (`choose_centroids`)**: Selects centroids for each crop type based on the ground truth.

