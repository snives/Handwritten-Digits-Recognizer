# Handwritten-Digits-Recognizer
## Demonstrate a neural network recognizing handwritten digits

The purpose of this demonstration is to train a neural network to recognize various handwritten digits and to correctly identify them as numbers.
This forms the basis of several technologies in widespread use such as OCR (Optical Character Recognition) used by the postal system, automated form
reading systems, automated check clearing in finance (read scanned checks routing numbers and dollar amounts), and even in your phone when you swipe text located in an image.

The neural network described in this repo, is based on Scikit-Learn's Multi-Layer Perceptron Classifier and is trained on 42000 28x28 grayscale images (MNIST).  
I use 5 fold cross-validation to maximize the training information while minimizing overfitting.
I performed hyperparameter optimization using the grid search method to identify an optimal neural network topology that neither underfits nor overfits the data.
This model achieves an accuracy of 97.1% 

## Sample Performance

### Input
![MNIST sample](https://raw.githubusercontent.com/snives/Handwritten-Digits-Recognizer/refs/heads/main/mnist%20sample.png)

### Output
|    |    |    |    |    |   |   |   |    |   |
|----:|----:|----:|----:|----:|----:|----:|----:|----:|----:|
|   1 |   0 |   1 |   4 |   0 |   0 |   7 |   3 |   5 |   3 |
|   8 |   9 |   1 |   3 |   3 |   1 |   2 |   0 |   7 |   5 |
|   8 |   6 |   2 |   0 |   2 |   3 |   6 |   9 |   9 |   7 |
|   8 |   9 |   4 |   9 |   2 |   1 |   3 |   1 |   1 |   4 |
|   9 |   1 |   4 |   4 |   2 |   6 |   3 |   7 |   7 |   4 |
|   7 |   5 |   1 |   9 |   0 |   2 |   2 |   3 |   9 |   1 |
|   1 |   1 |   5 |   0 |   6 |   3 |   4 |   8 |   1 |   0 |
|   3 |   9 |   6 |   2 |   6 |   4 |   7 |   1 |   4 |   1 |
|   5 |   4 |   8 |   9 |   2 |   9 |   9 |   8 |   9 |   6 |
|   3 |   6 |   4 |   6 |   2 |   9 |   1 |   2 |   0 |   5 |


```
Classification Report:

              precision    recall  f1-score   support

           0       0.99      0.99      0.99      4132
           1       0.99      0.99      0.99      4684
           2       0.99      0.95      0.97      4177
           3       0.98      0.97      0.97      4351
           4       0.99      0.98      0.98      4072
           5       0.99      0.97      0.98      3795
           6       0.99      0.98      0.99      4137
           7       0.97      0.99      0.98      4401
           8       0.96      0.99      0.97      4063
           9       0.99      0.93      0.96      4188

   micro avg       0.98      0.97      0.98     42000
   macro avg       0.98      0.97      0.98     42000
weighted avg       0.98      0.97      0.98     42000
 samples avg       0.97      0.97      0.97     42000
```



## Future Improvements

A higher accuracy could be obtained by using a (CNN) convolutional neural network which should be able learn higher order features.

Other concepts to employ would be to perform affine transformations to the training data to increase the diversity of the figures 
and further refine the networks generalizable understanding of numeric representations.








