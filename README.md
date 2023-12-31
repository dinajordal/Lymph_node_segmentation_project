# Lymph Node Segmentation project
## Overview
This project aimed to develop a machine learning model based on the U-net structure to segment lymph node units on whole slide images (WSIs) accurately. The model contributes to biomedical diagnosis and prognosis, particularly of various cancer types, such as skin and breast cancer. The algorithm utilizes the U-net architecture and follows a supervised machine-learning approach to achieve accurate segmentation.

## Technologies used
The machine learning architecture is based on the U-net architecture for its ability to segment medical images effectively. The choice of a supervised machine learning approach facilitates the training of the model using annotated datasets. The codes were developed with Python and libraries such as TensorFlow and OpenCV, which are employed for data processing, model training, and evaluation. The data preprocessing codes were written in Jupyter Notebook, whereas the machine learning training and testing were performed with the Google Collab Pro version.

## Project Steps
Most of the project was spent preparing the dataset for training, validation, and testing. The codes labelled 1-6 were used to process the data before training the model. Hyperparameter tuning was performed, and validation data was used for predictions. Finally, the machine learning model with the best performance on the validation dataset was compared to a simple contouring algorithm (developed without machine learning applied). This simple Python algorithm is part of a bigger machine-learning pipeline that aims to look at morphological changes within lymph nodes from breast cancer patients.

Counouring of lymph nodes: Each WSI was contoured, filtered and selected to obtain corresponding binary masks. 

Annotation Extraction: Manual annotations were performed with QuPath software and used to create binary masks.

Data Augmentation: Augmentation techniques are applied to increase the diversity of the training dataset.

Model Training: The U-net model is trained on the preprocessed and augmented dataset.

Model Evaluation: The trained model is tested and evaluated using validation datasets and hyperparameter tuning.

Model testing: The final model was tested against a ground truth test annotated by a certified pathologist and evaluated using dice score metrics.

### Challenges Faced
The primary challenges encountered during the project included:

**Data Preparation:** A significant amount of time was dedicated to preparing the dataset for effective model training, validation, and testing.
**Hyperparameter Tuning:** Fine-tuning model hyperparameters to achieve optimal performance requires careful experimentation and testing.

### Future Features

The project aims to implement the following features in the future:

**Integration with Existing Algorithm:** Integrating the developed lymph node segmentation model with an existing algorithm such as SmuLymphNet.

**Extended Cancer Types:** Adapt the model for the segmentation of lymph nodes in a broader range of cancer types beyond breast cancer.

________________________
Feel free to explore the codebase and contribute to the advancement of lymph node segmentation in biomedical research!
