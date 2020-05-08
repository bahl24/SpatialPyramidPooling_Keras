# Object Detection using Spatial Pyramid Pooling (SPPNet)
This is a Keras implementation of the object detection & classification algorithm described in the ECCV 2014 paper **"Spatial Pyramid Pooling in Deep Convolutional Networks for Visual Recognition"**. This has been done on top of AlexNet architecture using Keras API & Tensorflow.

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
