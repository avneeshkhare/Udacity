# AI Programming with Python Project

Image classification (102 flower categories) using Pytorch models.

Project code for Udacity's AI Programming with Python Nanodegree program. In this project, code developed for an image classifier built with PyTorch, then converted into a command line applications: train.py, predict.py.

The image classifier to recognize different species of flowers. Dataset contains 102 flower categories.

In Image Classifier Project.ipynb Densenet121 from torchvision.models pretrained models was used. It was loaded as a pre-trained network, based on which defined a new, untrained feed-forward network as a classifier, using ReLU activations and dropout. Trained the classifier layers using backpropagation using the pre-trained network to get the features. The loss and accuracy on the validation set were tracked to determine the best hyperparameters.

Command line applications train.py and predict.py

For command line applications there is an option to select either Alexnet or Densenet121 models.

Following arguments mandatory or optional for train.py:
'data_dir'. 'Provide data directory. Mandatory argument', type = str
'--save_dir'. 'Provide saving directory. Optional argument', type = str
'--arch'. 'Alexnet can be used if this argument specified, otherwise Densenet121 will be used', type = str
'--lrn'. 'Learning rate, default value 0.002', type = float
'--hidden_units'. 'Hidden units in Classifier. Optional argument', type = int
'--epochs'. 'Number of epochs. Default = 7', type = int
'--GPU'. "Option to use GPU (cuda)", type = str

Following arguments mandatory or optional for predict.py:
'image_dir'. 'Provide path to image. Mandatory argument', type = str
'load_dir'. 'Provide path to checkpoint. Mandatory argument', type = str
'--top_k'. 'Top K most likely classes. Optional', type = int
'--category_names'. 'Mapping of categories to real names. JSON file name to be provided. Optional', type = str
'--GPU'. "Option to use GPU (cuda)", type = str
