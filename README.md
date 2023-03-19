# EuroSat-Dataset-Classification


Constraints of the current solution : 

- Imbalanced classes: It appears that the model has difficulty distinguishing between certain classes, such as Pasture and Industrial. This may be due to imbalanced class distributions, where certain classes have significantly fewer samples than others. This can cause the model to be biased towards the majority classes and perform poorly on minority classes.

- Lack of regularization: The current model architecture does not include any regularization techniques such as dropout or weight decay, which may lead to overfitting on the training set and poor generalization performance on new data.

Potential improvements to the solution : 

- Increase the number of training epochs: my model is underfitting, meaning it is not able to capture the complexity of the data, I may need to train it for longer. I can try increasing the number of training epochs and see if that improves the performance on the validation set.

- Use data augmentation: Data augmentation can be used to increase the size of the training set by generating new samples from the existing ones. This can help the model learn more robust features and improve its performance on the validation set. I can use the ImageDataGenerator class in Keras to apply data augmentation techniques such as rotation, zooming, and flipping.

- Use a pre-trained model: I can use a pre-trained model such as VGG16 or ResNet as a feature extractor and train a new classifier on top of the extracted features. This can often lead to better performance on the validation set.

- Tune the hyperparameters: The performance of the model can be highly sensitive to the hyperparameters used during training. I can try adjusting the learning rate, batch size, optimizer, and other hyperparameters to see if that improves the performance on the validation set.
