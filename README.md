Classifying Paintings based on Movement
======

## Features
### Texture Descriptors
1. ~~Histogram of Oriented Gradients (HOG)~~
2. Pyramidal HOG (pHOG)
    * Same as HOG, implemented on 4 levels of a Gaussian Pyramid
3. Color HOG (cHOG) 
    * HOG implemented on each color plane of RGB color space
4. ~~Local Binary Pattern (LPB)~~
    * *Note: Paper uses 3x3 neighbourhood and limited to 58, we are currently using a radius of 8 and limited to 24*
5. Pyramidal LBP (pLBP)
    * LBP implemented on 4 levels of a Gaussian Pyramid
6. Local Invariant Order Pattern (LIOP)
    * Use VFLeat implementation *Note: Paper used VFLeat implementation of HOG and LBP also*
7. Edge Histogram Descriptor (EHD)
    * Use BilVideo-7 implementation
8. Spatial Envelope (GIST)

### Color Descriptors
1. Discriminative Color Names (DCN)
    * *Note: Paper mentions that they have used **author provided code** and gives the Painting-91 paper as a reference*
2. Color Structure Descriptor (CSD)
    * Use BilVideo-7 library to compute a 64 long CSD vector
### Miscellaneous
1. Bag of Words over SIFT keypoint descriptor
2. Gabor filters 
3. Scene Composition based on Gestalt Frameworks

--------

## Classifiers

### Mentioned in the Paper
1. Random Forest
2. SVM
3. 1-NN
4. 3-NN
5. 7-NN
6. Deep Convolutional Neural Network (MatConvNet library and LeNet architecture)

### Classifers currently used

1. KNN(3)
2. NuSVC
3. Linear SVC
4. Decision Tree 
5. Random Forest
6. AdaBoost Classifier
7. Gradient Boosting Classifier
8. Gaussian Naive Bayes
