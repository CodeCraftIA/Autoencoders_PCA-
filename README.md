This project explores the use of autoencoders and Principal Component Analysis (PCA) for dimensionality reduction and image reconstruction tasks using the MNIST dataset. Autoencoders are employed to reconstruct images of the same and next digits, comparing their performance against a Multilayer Perceptron (MLP) classifier. PCA is also used for image reconstruction across different numbers of principal components.

# Key Components:

# Data Handling and Preparation:
MNIST dataset is loaded and normalized.
Custom datasets are created for reconstructing images of the same and next digits based on original MNIST data.

# Autoencoder Implementations:

# Simple Autoencoder (My_Autoencoder1): 
Basic architecture with one encoding and one decoding layer. It reconstructs images of the next digit with varying accuracy.

# Complex Autoencoder (My_Autoencoder2): 
More layers in both encoding and decoding sections, improving reconstruction accuracy for next digits but showing mixed results for same digits.

# PCA Implementation (My_PCA):
Images are reconstructed using PCA with varying numbers of principal components.
Performance is evaluated by reconstructing images and testing them with an MLP classifier.

# Evaluation with MLP:
An MLP classifier trained on original MNIST data is used to evaluate reconstructed images' recognition accuracy.

# Results:
Autoencoders: The complex autoencoder performs better in reconstructing images of the next digit but worse for the same digit compared to the simple autoencoder.
PCA: Maintains high accuracy (>98%) with a high number of components but drops significantly with fewer components, demonstrating its sensitivity to the number of features retained.
