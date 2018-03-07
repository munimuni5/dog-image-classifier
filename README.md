# Dog Classification
39 and Canine is a project that uses [Google's Inception v3 model](https://storage.googleapis.com/download.tensorflow.org/models/inception_dec_2015.zip) with Tensorflow along with Django as a server to create a web interface to allow users to upload a photo of a dog for breed classification (the model has been trained with ~120 breeds).
The web interface is made using [materializecss](http://materializecss.com/) and [jQuery](https://jquery.com/)
It is extension of [this](https://github.com/DeepBlueCitzenService/Tensorflow-Server) project and the Django server is based on [this](http://tf-classify.herokuapp.com/classify_image/classify/) project's, which can be found [here]() on github.

## Live Site:
[39andCanine](http://thirty9andcanine.herokuapp.com/)

## Created Using:
* TensorFlow's tutorial for image classification neural network
* Stanford's collection of dog images [http://vision.stanford.edu/aditya86/ImageNetDogs/](http://vision.stanford.edu/aditya86/ImageNetDogs/)

## Using Retrained Inception Model
* Retrain the model using your images. Refer [here](https://www.tensorflow.org/tutorials/image_retraining).
* Fork and clone this repo
* Replace the generated graph and label files in `/classify_image/inception_model/`
* Check the views.py file to ensure that the final result model name is correct (it currently reads final_result:0--this is determined by your tensorflow project)
* Deploy the Django project on heroku or a similar platform
