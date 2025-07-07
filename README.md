# Handwritten-Digits-Recognizer
## Demonstrate a neural network recognizing handwritten digits

The purpose of this demonstration is to train a neural network to recognize various handwritten digits and to correctly identify them as numbers.
This forms the basis of several technologies in widespread use such as OCR (Optical Character Recognition) used by the postal system, automated form
reading systems, automated check clearing in finance (read scanned checks routing numbers and dollar amounts), and even in your phone when you swipe text located in an image.

The neural network described in this repo, is based on Scikit-Learn Multiclass is trained on 42000 28x28 grayscale images (MNIST).  
I use 5 fold cross-validation to maximize the training information while minimizing overfitting.
I performed hyperparameter optimization using the grid search method to identify an optimal neural network topology that neither underfits nor overfits the data.
This model achieves an accuracy of 97.1% 

## Sample Performance


## Future Improvements

A higher accuracy could be obtained by using a (CNN) convolutional neural network which should be able learn higher order features.

Other concepts to employ would be to perform affine transformations to the training data to increase the diversity of the figures 
and further refine the networks generalizable understanding of numeric representations.








