# Tensorboard

It is easy to get Tensorboard callbacks when you train your model through fit_generator() function.
But in this implementation where I trained a model, you train a Faster RCNN through train_on_batch() function.

Please open https://github.com/Janzeero-PhD/Faster_RCNN_roofs/blob/master/train_frcnn.py
I left comments "for Werner:" for you to find places in code where I want to insert functions for enabling Tensorboard callbacks.

I did it according to these steps: https://stackoverflow.com/questions/44861149/keras-use-tensorboard-with-train-on-batch

Additional information is here:
![ex1](https://i.imgur.com/DvDuQRf.jpg)

But error still exists and I cannot run train_frcnn.py file.


# Class activation heatmap

I want to have these maps for the last convolutional layer like here: https://github.com/jacobgil/keras-grad-cam

I cannot do that since during training I produce only model weights. I don't have separate file with model, since it is located in all these files of repo. You can find resnet.py file with CNN implementation, and find that nn_base() is that transfer learning part of Resnet which is passed to our Faster RCNN classifier (see train_frcnn.py). 

How to get classification maps from some layers of this nn_base()? 



