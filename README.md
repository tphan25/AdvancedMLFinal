# AdvancedMLFinal
Final project, evaluating models in Advanced ML for Depth Map Prediction

## To Run
In each directory there is a respective Jupyter notebook that needs to be run. For the monodepth folder, you need to run this jupyter notebook using python3.7, while for the Multi-Scale
folder, you'd be able to run 3.7 or any later version. There are instructions at the top of each python notebook for how to retrieve the data and models. For monodepth, the commands preceded
by ! in the first few cells should install the required data and model weights that we use in evaluation. For the Multi-Scale model, you will also have to retrieve the weights
online and move them into that directory - the instructions are all in the Jupyter notebooks themselves.

Each notebook will install all needed dependencies using pip in the first cell, and then the data in the next few cells. Then, it will bring the model into memory, and run an evaluation
on the first 200 images of the NYU Depth Dataset installed, and calculate the root mean squared error for each depth calculation (where depth is normalzed from 0-255 for every pixel in an image).
You will see the results printed on the last line of the notebook for both, which is just the root mean squared error - Multi-Scale should be more effective.

## Credits
I did not personally implement and train the models. My hardware would definitely not support training any neural network model to this level of complexity, so I took pretrained
models from the following repositories which are based off of the papers I evaluated: https://github.com/mrharicot/monodepth, and https://github.com/DhruvJawalkar/Depth-Map-Prediction-from-a-Single-Image-using-a-Multi-Scale-Deep-Network.
This project is not meant to be used for any commercial purpose, but only as a light demonstration of running these models against sample images and making depth map predictions, for a school project.
