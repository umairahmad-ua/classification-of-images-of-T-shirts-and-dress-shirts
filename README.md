# classification-of-images-of-T-shirts-and-dress-shirts
We have given 12000 training examples of shirts and t-shirts as a grey scale images, I have extracted  the feature by applying state of the art edge detection technique which is known as Canny dge  detection, because for this problem we don’t have any need to understand the inside edge features  color, size, and object inside but only the edge boundaries are enough to understand either its shirt or  t-shirt. 

I have also implemented the Histogram of Oriented Gradients (HOG) is a feature explainer mostly  used in image processing and computer vision for object detection. This technique counts occurrences  of gradient orientation in localized portions of an image. For this problem object is detected and  features are extracted via gradient. We will see the difference and performance of both techniques but  before that here is the examples of how extracted features may look alike

# Classification Techniques
I have used the three classifiers for this problem

  Random forest
  
  AdaBoost
  
  SVM
  
 # Hyper parameters for Canny and HOG
 Hyper parameters used in canny is sigma value the more sigma plays the role of a scale parameter for the 
edges, large values of sigma produce coarser scale edges and small values of sigma produce finer scale 
edges. Larger values of sigma also result in greater noise suppression.

After 5-fold cross validation the best value of sigma is 1
Hyper parameters used in HOG orientation and pixels per cell and pixels per block after 5-fold cross 
validation the best value of 

 Orientation is 9 

 Pixels per cell is 2

 Pixels per block is 2


# Performances on 5 fold
I have trained the model on three classifiers mentioned above after optimizing the value of lambdas (No 
of tress in adaboost, random forest and the C in SVM) and other hyper parameters sigma, orientation, 
pixels per cell and block 


# I am expecting test accuracy between 0.80-0.85 as shown in the above mean results and also in 67-33 split
