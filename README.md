# Object Detection using Spatial Pyramid Pooling (SPPNet) (paper id: 74)  
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
![image](https://user-images.githubusercontent.com/43816495/82816175-48c0fe00-9eb8-11ea-92da-1c41fc9ff034.png)


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
2. Open up ```sppnetFinal2.ipynb``` on google colab to run the respective experiments
3. Run code to obtain the result.  
  
**detection results will be obtained for test cases:**  
![image](https://user-images.githubusercontent.com/43816495/82817828-4d3ae600-9ebb-11ea-8344-a2af6c176d04.png)
![image](https://user-images.githubusercontent.com/43816495/82818038-b589c780-9ebb-11ea-81b2-f8645e1b1ceb.png)
![image](https://user-images.githubusercontent.com/43816495/82817955-896e4680-9ebb-11ea-876d-95890b42d8f4.png)  
## Obtaining mean Average Precision
In The Paper the mAP is 35.11% in the testing set.  
After executing ```sppnetFinal2.ipynb``` **Ground Truth** and **Detected values** will be stored (we ran for 500 images due to out of memory issue) in your drive.  
You can run the code for all images by removing size restruction on read_images_for_detection      
```input_imgs, region_proposals, out,no_of_proposals, gt_boxes = read_images_for_detection(df_anno, list_of_img_name, img_dir)```

- Copy ground-truth files into the folder input/ground-truth/ 
- Copy detection-results files into the folder input/detection-results/
- Run the code: ```python mainmAP.py```  
  
**mAP output can be viewed in output folder** 
![detection-results-info](https://user-images.githubusercontent.com/43816495/82814541-fe8a4d80-9eb4-11ea-8fa4-133f2c742134.png)
![mAP](https://user-images.githubusercontent.com/43816495/82815095-0eeef800-9eb6-11ea-9231-620d2b671591.png)  
**Average Precision for diningTable is shown below . For rest of classes it can be found in output folder**  
![diningtable](https://user-images.githubusercontent.com/43816495/82815110-19a98d00-9eb6-11ea-9c72-c69234825857.png)
