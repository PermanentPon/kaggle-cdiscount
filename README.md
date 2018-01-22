## [Cdiscount’s Image Classification Challenge](https://www.kaggle.com/c/cdiscount-image-classification-challenge)
This is my solution for Cdiscount’s Image Classification Challenge on Kaggle. The main idea was to train two models on disjoint data. The first model was trained on the first images of products and the second one on all other images. After that, the resultant resulting output was used to build an FC net for final classification.
## Result
Public LB - 151st place (top 25%)
## Structure
5 notebooks:
1. BSON to files - generates folders with images from bson files
2. Image  augmentation & over-under sampling - augments and adds images in classes with small number of images and delete images in categories with too many images.
3. Keras modeling from files - traines models from files
4. Testing base models and ensembles - code to test trained models and make ensembles of models
5. Train and test 2_layers_FC on top - creates a new FC net on top of features from last layer of the base CNN for all images of products (from 1 to 4 images)
## How to use
Run all the cells in all the files one by one from 1 to 5.
