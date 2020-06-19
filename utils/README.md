# utils

## Rhino + Grasshopper Files:

...  

## Python Notebooks:

All of these notebooks are designed to run in Google Colaboratory

#### Dataset Augmentation
Loads a set of images, and uses the Augmentor python package to sample a larger set of paired images to train the model with. This notebook is designed to load and save images from locations in Google Drive, but you could also run it locally with a tool like `Jupyter Notebook` and skip the cells that connect to Google Drive.

#### Pix2Pix - Model Training
This is the source code for the pix2pix model architecture provided by the Tensorflow team. The original pix2pix tensorflow implentation was re-written in Tensorflow 2.0. This notebook cuts out most of the notes and diagrams, so if you'd like to learn more about how the code works, I'd recommend looking at the [original version](https://www.tensorflow.org/tutorials/generative/pix2pix).

### Pix2Pix - Load Saved Model
The previous notebook will save an `.h5` file after training is complete. This is the format we can use to upload checkpoints to the RunwayML model. If you'd like to test the model before moving on, this notebook can be used to test the saved checkpoint. Just update the `MODEL_PATH` variable to point to the location where training notebook saved your `.h5` file, and update the `TEST_IMAGE` variable to load an image to send through the model.