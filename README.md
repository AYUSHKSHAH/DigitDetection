# Street View Housing Number Digit Recognition
## Problem Statement
Recognizing multi-digit numbers in photographs captured at street level is an important 
component of modern-day map making. A classic example of a corpus of such street
level photographs is Google’s Street View imagery composed of hundreds of millions 
of geo-located 360-degree panoramic images.

The ability to automatically transcribe an address number from a geo-located patch of 
pixels and associate the transcribed number with a known street address helps 
pinpoint, with a high degree of accuracy, the location of the building it represents. More 
broadly, recognizing numbers in photographs is a problem of interest to the optical 
character recognition community.

While OCR on constrained domains like document processing is well studied, arbitrary 
multi-character text recognition in photographs is still highly challenging because of 2 primary reasons: 
1. There is a wide variability in the visual appearance of text in the wild on account 
of a large range of fonts, colours, styles, orientations, and character arrangements.
2. Environmental factors such as 
lighting, shadows, specularities, and occlusions as well as by image acquisition factors 
such as resolution, motion, and focus blurs further complicates the scenario.

This project aims to detect the prominent number in each image in a subset of the actual data ([Full data from source](http://docs.h5py.org/en/stable/high/dataset.html ))

## Domain
Autonomous Vehicles, Neural Networks

## Project Steps
-  Use the Street View Housing Number (SVHN) dataset subset
-  Reshape and Normalize the data properly into a 2D tensor for ANN instead of 3D
-  One Hot Encode the targets
- Build a Custom Architecture using Keras and Tensorflow using appropriate activation functions and categorical cross-entropy as the loss function
- Hyperparameter tune the model to increase the training and validation accuracy and prevent overfitting

