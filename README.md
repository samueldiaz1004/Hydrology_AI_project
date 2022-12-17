# Camera-based Water Stage and Discharge Prediction with Machine Learning

<p align="center">
  <img src="https://user-images.githubusercontent.com/71342016/208263381-18084202-96fe-4ea0-aeed-4ef29920a811.jpg" width="350" />
  <img src="https://user-images.githubusercontent.com/71342016/208263383-03a21b1a-2922-437c-8918-067bc1d9b194.png" width="350" /> 
</p>

## Objective
Find a model that predicts the stage and discharge of water in a body of water through the use of a numeric database and images of the site from the same angle over the years.

## Database Content
The numeric database was divided into two types of data, generic and hand-crafted (57 independent variables). The second database contains all the images that were used to get the information for the former dataset.

## Models
For the numeric database the implemented models were variations of:
* [MLP Regressor](https://en.wikipedia.org/wiki/Multilayer_perceptron)
* [KNN Regressor](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm#k-NN_regression)
* [Random Forest Regressor](https://en.wikipedia.org/wiki/Random_forest)

And for the images the implemented models were variations of:
* [CNN](https://en.wikipedia.org/wiki/Convolutional_neural_network)
* [MLP Regressor with Segmentation](https://towardsdatascience.com/segmentation-based-interpretability-of-cnn-classification-6de02f9a8303)

## Conclusion and Future Work
The best models consistenly were the CNN and versions of the MLP Reggresor, MLP Regressor with data from Segmentation having a slight edge over the others. To prove the complete effectiveness of the selected model it is theorized that it will require around 100 segmentation mask.

## Development
Detailed information of the project can be found in the `Research_paper.pdf` file and implementation of the algorithms in the `models` directory.

## Requirements
* A recent version of Python3 with pip to install libraries like TensorFlow and Keras
* Jupyter server environment
