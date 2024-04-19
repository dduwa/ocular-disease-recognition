# Computer-Aided Multi-Class Ocular Disease Recognition System
Within this repository, there is implementation of a multi-class medical image classification system using various CNN architectures. A collection of 5000 colour fundus photographs of distinct ocular diseases can be found within the ODIR-5K dataset. The are 8 labels that can be allocated to the patients in this dataset - 
- Normal (N)
- Diabetes (D)
- Glaucoma (G)
- Cataract (C)
- Age related Macular Degeneration (A)
- Hypertension (H)
- Pathological Myopia (M)
- Other diseases/abnormalities (O)
The dataset has only been majorly explored using binary classification due to its class imbalance - multi classification has been used with multiple explainability techniques to resolve the issue of transparency in automated medical diagnosis by addressing the reasoning behind the decisions of highly accurate computer aided diagnositic systems. 

and the dataset ODIR-5K.

Link of ODIR5K - https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k 

The following keras pretrained models have been used, they have been listed below in order of best performing model on image classification accuracy and precision: 
1. VGG16
2. VGG19
3. Xception
4. ResNet50
5. Inception

To run the code for each model, a kaggle.json file is required to be downloaded into the notebook to access the dataset. This has been attached in the repository. 

There is also implementation of explainable AI but only in the best performing model - which is VGG16. 
