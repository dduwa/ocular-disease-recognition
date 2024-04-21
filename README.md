# Computer-Aided Multi-Class Ocular Disease Recognition System

## Introduction
This repository houses an innovative multi-class medical image classification system designed to advance the diagnosis of various ocular diseases through the power of Convolutional Neural Networks (CNN) and transfer learning. Utilizing the ODIR-5K dataset, which comprises 5000 color fundus photographs representing a range of ocular conditions, our system aims to classify these into eight distinct categories: Normal (N), Diabetes (D), Glaucoma (G), Cataract (C), Age-related Macular Degeneration (A), Hypertension (H), Pathological Myopia (M), and Other diseases/abnormalities (O).

Addressing the common challenge of class imbalance in medical image datasets, our approach embraces multi-class classification enhanced with various explainability techniques. This methodology not only improves diagnostic accuracy but also increases transparency, enabling healthcare professionals to understand the rationale behind each diagnosis made by our computer-aided diagnostic system.

## Features and Technologies Used
### Dataset
- **ODIR-5K Dataset:** A comprehensive collection of 5000 color fundus photographs, accessible on Kaggle [here](https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k/suggestions?status=pending&yourSuggestions=true).

### Models Employed
The following pre-trained models from Keras were used, selected for their proven efficiency in image classification tasks:
- VGG16
- VGG19
- Xception
- ResNet50
- InceptionV3

These models were chosen based on their performance metrics, including accuracy and precision, in classifying images into the relevant ocular disease categories.

## Getting Started

### Prerequisites
Before starting, ensure you have:
- A Kaggle account for dataset access
- Google Colab for running notebooks

### Installation and Setup
1. **Clone the repository:**
```bash
git clone https://github.com/dduwa/ocular-disease-recognition-system.git
```
2. **Access the ODIR-5K dataset:** Navigate to the provided Kaggle link and download the dataset.
3. **Prepare the kaggle.json file:** Follow the instructions on Kaggle for generating and downloading your API key (kaggle.json). This file is crucial for accessing the dataset from within the notebooks. There is also a kaggle.json file already available for use aswell in the repository

### Running the Models: 
1. **Open the notebooks on Google Colab:** Import the cloned notebooks into Google Colab to utilise its computational resources and pre-installed libraries.
2. **Upload kaggle.json:** Ensure the kaggle.json file is uploaded to the Colab environment using the section "Access Dataset via Kaggle API" to programmatically download the dataset.
3. **Run the notebooks:** Follow the step-by-step instructions within each notebook to train and evaluate the models. The notebooks are self-contained and include comments to guide you through the process.

## Explainability AI (XAI) Techniques 
To enhance the transparency of the model predictions, there is implementation of XAI techniques for the top performing model which is VGG16. These techniques are designed to provide insights into the decision-making process of the neural network, thereby making the outcomes more interpretable for medical professionals. To run the XAI implementations please upload the images within the **XAI Test Images** folder to the Colab environment. 
