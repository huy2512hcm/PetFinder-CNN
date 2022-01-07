# Convolutional Neural Networks project

In my final project, I participated in Kaggle's Pawpularity Contest. 

A Malaysia’s leading animal welfare
platform, PetFinder.my, proposes that cuter images of rescued stray animals will increase the chance of
faster adoption. To help people better photo the rescued pets, PetFiner.my provides a cuteness calculator
on their webpage to evaluate how cute the images are, so that pet photographers can work toward photos with
higher cuteness score. Besides the existing cuteness algorithm, PetFinder.my wants to explore the possibility
of machine learning methods on scoring pet images, as machine learning models with high capacity may find
details and hidden correlations not obvious to human eyes.

Task, as described in the challenge: _‘you’ll analyze raw images and metadata to predict the "Pawpularity"
of pet photos. You’ll train and test your model on PetFinder.my’s thousands of pet profiles.'_

Link: https://www.kaggle.com/c/petfinder-pawpularity-score

For this challenge, I believe that Convolutional Network is the network architecture that made the most sense here because we are predicting using images. 
I use Convolution layers to extract the features from the images. I also use ReLU activation since the image pixel is bigger than 0, together with MaxPool, BatchNorm2d, Dropout2d, and Linear as the layers using PyTorch packages. From the competition’s discussion, there are some suggestions to use linear regression model combined with deep learning on metadata in order to achieve better score.

In this contest, I also try out the Linear models and Ensemble Models approaches, but didn't get a good result. The reason may be due to the complication of the problem that the metadata with just 12 features is certainly not enough to predict the attribute (e.g pawpularity) of an image compared to training using the image itself. 
