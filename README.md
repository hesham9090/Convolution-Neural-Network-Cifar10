# Convolutional Neural Networks Cifar10 Classification.


## Task 1

### Build a CNN with three convolution layers with feature maps 25, 50, and 100 respectively with kernal size equal 2*2.
Each convolution layer will be followed by an relu function and a max pool layer with pool size 2\*2.

### (A)
1. Use Cifar10 Dataset `keras.datasets.cifar10`
2. Train the CNN for 10 epoch on `CIFAR10` dataset only on classes from 0 to 4
3. plot training & validation loss.


### (B)
1. Increase the number of epochs to 30 and plot the new training and validation loss curves
2. Test the model (with 30 epochs) on the test set and write the average tetsing accuracy
3. Now, augument the test images for class 1 (using flip left to right augumetation) and then test the CNN on the test dataset for class 1 and write the average testing accuracy
4. Apply the same augumentation on the training dataset for class 1, and add these augumented images to the training dataset, 
retrain the model for 30 epocs, then test it again on the augumented test images for class 1 you created on the previous step
5. Discuss the change in the accuracy between 3 & 4




## Task 2

### (A) 
1. Re-Use the last model from question 1 at point B.1 to classify CIFAR images with classes 5 to 9. Freeze all layers except 
the last one and replace it by new Softmax and run the new model for 30 epochs.
2. Plot the training and validation loss curves.
3. Unfreeze the last convolution layer (and its pooling layer) then train again on classes 5 to 9 for 30 epochs.
4. Plot the new training and validation loss curves.

### (B) 
1. Add a forth convolution layer with 200 features maps to the model that you created in step A.1 and retrian the model for 30 epochs
2. Plot the training and validation loss curves.

### (C) 
1. Write your comments on the performance by comparing steps A.4 & B.2
