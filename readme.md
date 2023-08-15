# Deconstructive vs. Tudor

This model can clasify a tudor style building, which is a more old style of building, and can also classify a deconstructive style building, which falls into the more modern category. I decided on this topic for the project because I found it interesting how the model classified the building based on the qualities of that of the building.

![add image descrition here](direct image link here)

## The Algorithm

The is a resnet-18 model that was ran with the Jetson-Nano and trained using a large data set of deconstructive and tudor images. It uses imagenet.py to tell the difference between the two styles.

## Running this project

1. You will need to have the Jetson Inference Library and python3 installed
2. Download the model (https://github.com/JoshIgnatin/deconstructiveVsTudor/tree/master/models)
3. Download data set (https://drive.google.com/drive/folders/1Zsk8jYITbgg2i4KAmU-SSPL1c8yAyIXQ?usp=sharing)
4. Go into your command line (terminal, vs code, etc.)
5. Locate the classification directory
```$ cd jetson-inference/python/training/classification```
6.

[View a video explanation here](video link)
