# Face recognition CNN deep neural network and LBP approach

## Two approaches for implementation

1. CNN based
2. LBP feature extraction + classification with SVM and kNN

## 1. CNN

Procedure:

1. Load faces dataset
2. Preprocessing (normalization and reshaping images)
3. Split train and test datasets
4. Architecture: 
        * Convolotional layer (2 convolutional layers)
        * pooling layer (max pooling)
        * Fully connected layer (dense with ReLu + dropout layers) and softmax as the last layer
5. Training the model
6. Evaluation of the model
7. Plot visualizations


## 2. LBP + classification

1. Retrieve dataset (in our case `yale` dataset) for face recognition. (Available at http://vision.ucsd.edu/content/yale-face-database#:~:text=Synopsis,sleepy%2C%20surprised%2C%20and%20wink.)
2. Implement LBP algorithm for feature extraction (histogram)
3. Predict idenity based on features extracted from LBP using kNN and SVM
4. Find optimal values for number of points and radius in LBP
5. Plot visualizations