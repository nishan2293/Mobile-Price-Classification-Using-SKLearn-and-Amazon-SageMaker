# Project Report: Mobile Price Classification Using SKLearn and Amazon SageMaker

## 1. Introduction

### 1.1 Project Objective
The objective of this project was to develop a machine learning model capable of classifying mobile phones into different price ranges based on various features. The model was built using SKLearn and deployed using Amazon SageMaker to leverage its robust infrastructure for training, deployment, and real-time predictions.

### 1.2 Overview
Mobile price classification is an essential task in the retail and e-commerce industry. By accurately predicting the price range of a mobile phone based on its features, companies can make informed decisions regarding pricing strategies, inventory management, and market analysis.

## 2. Data Description

### 2.1 Dataset
The dataset used for this project contained the following features for each mobile phone:
- Battery Power
- Bluetooth Support
- Clock Speed
- Dual Sim Support
- Front Camera Megapixels
- 4G Support
- Internal Memory
- Mobile Depth
- Mobile Weight
- Number of Cores
- Primary Camera Megapixels
- Pixel Resolution Height
- Pixel Resolution Width
- RAM
- Screen Height
- Screen Width
- Talk Time
- 3G Support
- Touch Screen Support
- Wi-Fi Support
- Price Range (Target Variable)

The dataset was split into training and testing sets to evaluate the model's performance.

## 3. Methodology

### 3.1 Data Preprocessing
Data preprocessing steps included handling missing values, normalizing features, and splitting the dataset into training and testing sets.

### 3.2 Model Training
A RandomForestClassifier model was trained using the training dataset. The model was selected for its ability to handle classification tasks effectively and its robustness against overfitting.

### 3.3 Model Deployment
Amazon SageMaker was used for model deployment, providing a scalable and managed infrastructure. Key components included:
- **SageMaker Notebook Instances**: Used for data preprocessing, model training, and evaluation.
- **Training Jobs**: Executed on SageMaker to train the model with optimized configurations.
- **Endpoints**: Created for real-time predictions and integrated into the deployment pipeline.

### 3.4 AWS Services Utilized
- **S3 Buckets**: Used for data storage and management.
- **IAM Roles**: Implemented for secure access management.
- **CloudWatch**: Utilized for monitoring and logging training and deployment processes.

## 4. Results

### 4.1 Model Performance
The model achieved the following performance metrics on the test dataset:
- **Accuracy**: 88.33%
- **Precision**: 0.95 for class 0, 0.85 for class 1, 0.80 for class 2, 0.91 for class 3.
- **Recall**: 1.00 for class 0, 0.80 for class 1, 0.77 for class 2, 0.95 for class 3.
- **F1-Score**: 0.97 for class 0, 0.83 for class 1, 0.79 for class 2, 0.93 for class 3.

### 4.2 Visualizations
Key visualizations were generated to provide insights into model performance:
<img width="704" alt="image" src="https://github.com/nishan2293/Mobile-Price-Classification-Using-SKLearn-and-Amazon-SageMaker/assets/157925518/37125a17-56a7-4e73-8fc2-9d1f4dbf937c">

<img width="807" alt="image" src="https://github.com/nishan2293/Mobile-Price-Classification-Using-SKLearn-and-Amazon-SageMaker/assets/157925518/2c8ee647-dc8a-4d0d-b7e6-931a2135c7d3">

<img width="751" alt="image" src="https://github.com/nishan2293/Mobile-Price-Classification-Using-SKLearn-and-Amazon-SageMaker/assets/157925518/0494cbc3-91dc-4b9b-8eab-7dc6bce3373e">

<img width="823" alt="image" src="https://github.com/nishan2293/Mobile-Price-Classification-Using-SKLearn-and-Amazon-SageMaker/assets/157925518/44ea9ba4-b6b1-45b7-8e36-a8ea80deabe6">

<img width="822" alt="image" src="https://github.com/nishan2293/Mobile-Price-Classification-Using-SKLearn-and-Amazon-SageMaker/assets/157925518/2f53ea5b-666d-48a4-bc4b-42e7c1f86cd1">

## 5. Conclusion

### 5.1 Summary
The project successfully developed and deployed a machine learning model to classify mobile phone prices into different ranges with high accuracy and performance. The integration of Amazon SageMaker provided a scalable and efficient infrastructure for training and deploying the model.

### 5.2 Future Work
Future enhancements could include:
- Experimenting with different machine learning models and algorithms.
- Hyperparameter tuning to further improve model performance.
- Incorporating additional features to enhance the predictive power of the model.
- Extending the model to handle more complex classification tasks in the mobile phone domain.

## 6. Appendix

### 6.1 Code
The complete code for data preprocessing, model training, deployment, and visualization is provided in the accompanying Jupyter notebook and script files.
