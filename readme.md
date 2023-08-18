# Deconstructive vs. Tudor

This model can classify both Tudor-style buildings, which belong to an older architectural style, and deconstructive-style buildings, which fall under the more modern category. I chose this topic for the project because I found it fascinating to observe how the model categorizes these buildings based on their distinctive qualities.

![Tudor House](https://drive.google.com/file/d/1it-c41NFUDIiE5LgLg-WhdeSB62P1vAy/view?usp=sharing)

## The Algorithm

The is a resnet-18 model that was ran with the Jetson-Nano and trained using a large data set of deconstructive and tudor images. It uses imagenet.py to tell the difference between the two styles.

## Running this project

1. You will need to have the Jetson Inference Library and python3 installed
2. Download the model (https://github.com/JoshIgnatin/deconstructiveVsTudor/tree/master/models)
3. Download data set (https://drive.google.com/drive/folders/1Zsk8jYITbgg2i4KAmU-SSPL1c8yAyIXQ?usp=sharing)
4. Go into your command line (terminal, vs code, etc.)
5. Locate the classification directory:
```cd jetson-inference/python/training/classification```
6. Define the NET and DATASET variables:
```NET=models/arch```
```DATASET=data/arch```
7. Use this line to see how it does on a image (change "tudor/014059.jpg" to the example you want):
```imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/tudor/014059.jpg test1.jpg```
8. Open the file using the methods needed to view the result
9. You can inport your own images if you want to test them.

([Video Explanation](https://youtu.be/i_HZ5Vq8cGw))
