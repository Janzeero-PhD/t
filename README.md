# Keras Faster R-CNN for trees detection on abandoned city roofs

Implementation is adapted from https://github.com/kbardool/keras-frcnn.

Model is trained on the small dataset (~50 images) with data augmentation. Classification accuracy on validation data was 82 % (single class detection), RPN quality is relatively good. Classification accuracy on the test data is 70-80 % (will be specified).

The further plans are to enlarge number of epochs, play with sizes of images, collect a uniform and larger training dataset.

The examples of training images (without labels):

The examples of test results (with labels):
![ex1](https://i.imgur.com/DI82mlF.jpg)
