# Object Detection using Spatial Pyramid Pooling (SPPNet)
This is a Keras implementation of the object detection & classification algorithm described in the ECCV 2014 paper **"Spatial Pyramid Pooling in Deep Convolutional Networks for Visual Recognition"**. This has been done on top of AlexNet architecture using Keras API & Tensorflow.
![spp](http://i.imgur.com/SQWJVoD.png)

(Image credit: Spatial Pyramid Pooling in Deep Convolutional Networks for Visual Recognition, K. He, X. Zhang, S. Ren, J. Sun)

This is an implementation of both **object detection & classification** and has been trained and tested on **PASCAL VOC 2007 dataset**.

Paper: [Spatial Pyramid Pooling in Deep Convolutional Networks for Visual Recognition](https://arxiv.org/abs/1406.4729)

Dataset: [The PASCAL Visual Object Classes Challenge 2007](http://host.robots.ox.ac.uk/pascal/VOC/voc2007/)

## Dataset
PASCAL VOC 2007 dataset consists of 20 visual object classes from realistic scenes. These include - 
1. Person: person
2. Animal: bird, cat, cow, dog, horse, sheep
3. Vehicle: aeroplane, bicycle, boat, bus, car, motorbike, train
4. Indoor: bottle, chair, dining table, potted plant, sofa, tv/monitor

## Instructions to run
It is assumed that you have a working copy of Conda installed
```
git clone https://github.com/bahl24/SpatialPyramidPooling_Keras.git
cd SpatialPyramidPooling_Keras
conda env create -f environment.yml
conda activate base
jupyter notebook
```
1. Copy the data set to your drive [click here](https://drive.google.com/drive/folders/1FKYBjJ-ifct_bLFR6CSyNvbDswwo_B1X?usp=sharing)
2. Open up ```sppnetFinal2.ipynb``` to run the respective experiments

## Obtaining mean Average Precision
After executing ```sppnetFinal2.ipynb```**Ground Truth** and **Detected values** will be stored in your drive copy those:
- ground-truth files into the folder input/ground-truth/ 
- detection-results files into the folder input/detection-results/
- Run the code: ```python main.py``` 
