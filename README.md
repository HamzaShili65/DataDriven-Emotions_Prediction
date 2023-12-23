# Data Driven Speech Emotion Classification

## Overview
This project explores the application of machine learning in speech emotion classification. The goal is to classify speech clips into the correct emotion of the speaker using three different machine learning techniques: Support Vector Machines (SVM), Convolution Neural Networks (CNN), and Gaussian Mixture Modelling (GMM). I followed a comprehensive process of feature extraction, selection, preprocessing, training, validation, and testing for each method.

## Data Format and Feature Extraction
The dataset consists of sound files representing 8 different emotions. I focused on extracting features relevant to speech emotion recognition, such as frequency range, volume, and dynamic range. Specific features extracted include:
- Mel-frequency cepstral coefficients (MFCCs) for SVM and GMM
- Mel-Spectrogram bands for CNN implementation

These features were extracted using the Librosa Library and were chosen for their relevance to the audio signal's characteristics like pitch, timbre, and spectral envelope.

## Model Implementation and Selection
### Gaussian Mixture Model (GMM)
GMM was selected for its efficiency in capturing complex data distributions and its ability to identify clustering relationships in an unsupervised manner. Its strengths lie in quick execution and interpretability, while its limitations include assumptions about data distribution and feature independence.

### Support Vector Machine (SVM)
SVM was chosen for its effectiveness with high-dimensional data. The model's strengths include ease of implementation and handling of complex data. However, it is computationally expensive and primarily suited for binary classification.

### Convolution Neural Network (CNN)
The CNN model was implemented for its layer-specific feature learning capabilities, ranging from simple to complex structures within speech signals. Its main advantages are automatic feature detection and learning complex patterns, but it requires substantial computational resources and is prone to overfitting.

## Results and Conclusion
Each model presented unique strengths and challenges. The SVM model showed reasonable accuracy, especially after hyperparameter optimization. GMM faced challenges due to incomplete models for each emotion class, leading to inaccurate predictions. CNN, while quick and efficient, struggled with overfitting and achieved a best validation accuracy of 76.00% at epoch 5.

In summary, this project offered practical insights into choosing suitable models for specific tasks, balancing computational efficiency, and accuracy. Future work could involve exploring more features, cloud computing for enhanced performance, and improved implementation to achieve higher accuracy.

