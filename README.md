# KaggleInvasiveSpecies
Playing around with the Invasive Species Kaggle Competition


Quick first attempt at the Invasive Species Kaggle competition

This first approach takes a pretrained VGG model with added batchnorm and precomputes its outputs after a little bit of fine tuning.
Then we just pop on a couple of FC Dense layers and train with the precomputed outputs.


TODO:
* Data Augmentation
* Psuedo Labeling
* Take advantage of data leakage from different sized photos
* Add bounding boxes for ensemble models


I also want to test out adaptive stepwise learning rates beyond just simply using Adam
