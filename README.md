# KaggleInvasiveSpecies
Playing around with the Invasive Species Kaggle Competition


Quick first attempt at the Invasive Species Kaggle competition
After playing around a little bit, this got me in the top half of the leaderboard with a AUC of .96341 without ANY data augmentation!

This first approach takes a pretrained VGG16 model with added batchnorm and precomputes its outputs after a little bit of fine tuning.
Then we just pop on a couple of Fully Connected Dense layers and train with the precomputed outputs.


TODO:
* Data Augmentation
* Psuedo Labeling
* Take advantage of data leakage from different sized photos
* Add bounding boxes for ensemble models


I also want to test out adaptive stepwise learning rates beyond just simply using Adam
