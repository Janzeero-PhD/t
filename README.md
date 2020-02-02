# Keras Faster R-CNN for trees detection on abandoned city roofs

Implementation is adapted from https://github.com/kbardool/keras-frcnn.

Model is trained on the small dataset (~50 images) with data augmentation. Classification accuracy on validation data was 82 % (single class detection), RPN quality is relatively good. Classification accuracy on the test data is 70-80 % (will be specified).

The further plans are to enlarge number of epochs, play with sizes of images, collect more uniform and larger training dataset.

Please consider (my settings to run this model):
- Tensorflow version 1.15.0 (older);
- Keras version 2.0.5 (older);
- but CUDA is 10.0.
Probably CUDA should be 9.0. and this will not produce some discrepancies which I faced training this model on my GPU (RTX2060). Will check it later.


The examples of training images (without labels):
![ex1](https://i.imgur.com/hvuAXqK.jpg)
![ex2](https://i.imgur.com/Bit9W8K.jpg)
![ex3](https://i.imgur.com/ryhzdyj.jpg)



The examples of test results (with labels):
![ex4](https://i.imgur.com/DI82mlF.jpg)
![ex5](https://i.imgur.com/awBwlfj.jpg)
![ex6](https://i.imgur.com/J94a1aT.jpg)
![ex7](https://i.imgur.com/Fps6mrz.jpg)
![ex8](https://i.imgur.com/zXEjhsZ.jpg)
