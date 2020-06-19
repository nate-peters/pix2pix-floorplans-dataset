# pix2pix-floorplans-dataset

This repository contains all of tools necessary to recreate the models that were shown in the DigitalFutures 2020 workshop "INSERT TITLE"
This is a companion to the `pix2pix-runway` repo, which contains the code needed to run a pix2pix model locally in RunwayML

### About the data:

...  
The dataset is derived from images of floor plans for small, single-story houses sourced from HousePlans.com. Each image was manually tagged using Rhino and Grasshopper, and exported as an A/B image pair for use with pix2pix. The A image contains the boundary shape of each floor plan represented as a solid black region. The B image contains the same boundary, but with color coded regions that correspond to different room types in the plan.

![test](dataset/Augmented/Combined/0d565e4fb293.png)
...

### Organization of the `/dataset` directory:

This directory contains the images that we'll use to train a pix2pix model.
`./Source Images`: These are the source images that informed the room tags.  
`Original`: 
- `/A`: The boundary shape of each floor plan represented as a solid black region
- `/B`: The color tagged plans