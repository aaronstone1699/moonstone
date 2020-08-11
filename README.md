# moonstone

--RM--
This is the rishnet32x64x64x128 model which predicts the result of the test dataset

x.pickle contains contains the features of the training dataset 
y.pickle contains the respective labels

the preprocessing of the data for training includes :
resizing all the images to 128*128 size 
grayscaling the images
reshaping them as -1,128,128,1

The model uses keras sequential model with 4 convolution layers together with 4 pooling layers followed by dense and flatten layers,the activation for the conv laver is 
rectified linear and for final dense layer is a simple sigmoid function,the adam optimizer is used with loss as binary crossentropy
the model after 10 epochs results in a 99.987% accuracy and 0.0058 loss with a 99.996 validation accuracy
