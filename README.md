# TrafficSignsClassification
An end-to-end traffic sign classification system using a custom Convolutional Neural Network (CNN) built with TensorFlow/Keras. The workflow begins with automated ingestion of traffic-sign images organized by class folders, followed by dataset construction, exploratory visualization, and class-distribution analysis.


**Project Overview**

This project builds a complete Traffic Sign Classification System using a custom Convolutional Neural Network (CNN) developed with TensorFlow/Keras. The system automates dataset ingestion, preprocessing, augmentation, model training, evaluation, and model export.

**Key Features**

Automated dataset loading from class-labeled folders.
Training/Validation/Test split with integrity checks to ensure image–label consistency.
Comprehensive preprocessing, including:
Grayscale conversion
Histogram equalization
Normalization
Data augmentation pipeline using TensorFlow’s RandomTranslation, RandomZoom, and RandomRotation layers to enhance generalization.

**Custom CNN architecture featuring:**

Multiple convolutional/pooling layers
Dropout regularization
Fully connected classifier head
Training monitoring: loss and accuracy curves for both training and validation.
Model evaluation on a held-out test set to measure generalization performance.
Model export as a serialized .p (pickle) file for downstream inference or deployment.

**Workflow Summary**

Image Importing: Load all images and corresponding labels from the dataset directory.
Exploratory Visualization: Display sample images from each class and a bar chart of dataset distribution.
Preprocessing: Convert to grayscale, equalize lighting, normalize, and reshape for CNN input.
Augmentation: Apply real-time transformations to the training pipeline to reduce overfitting.
Model Training: Train the CNN using Adam optimizer and categorical cross-entropy loss.
Evaluation: Plot accuracy/loss metrics and test model performance.
Saving the Model: Store the trained model for future use.

**Output**

A trained traffic sign classifier model: model_trained.p

Performance plots for:
Training vs. validation loss
Training vs. validation accuracy
