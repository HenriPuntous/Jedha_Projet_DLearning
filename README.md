# Jedha_Projet_DLearning
Repo for ipynb notebook for Jedha final project

## Notebook synthesis
### 1 Data loading and preparation for input to Yolo
####         - Unzipping datasets from tar.gz format
####         - Load yoloV5
####         - Convert each annotation file with bounding box limits into .txt file per image, to input these into Yolo v5
####         - Sanity check of visualisation of several images with their associated bouding boxes, and confirm cracks are detected
####         - Creation of train, test, val sub folders for images and annotation
### 2 Model training
####         - Loading of YoloV5
####         - Choice of parameters for training ; here, for demo, only one epoch has been taken for WandB demo
####         - Sanity check of algo performance with WandB plots of Recall, Precision, Advanced Precision, 
### 3 Model deployement with GRadio
#####         - definition of interface to load one image and visaluize the associated cracks detected
### Dataset used for the training comes Global Road Detection challenge of 2020 ; it gathers data from Czech, Japan and India ; globally 20 000 photos and 35 000 annotations available
##### Original dataset in tar.gz could be downloaded via the links below ; dataset is split in train (images + annot), test (images), val (images)
##### https://mycityreport.s3-ap-northeast-1.amazonaws.com/02_RoadDamageDataset/public_data/IEEE_bigdata_RDD2020/train.tar.gz
##### https://mycityreport.s3-ap-northeast-1.amazonaws.com/02_RoadDamageDataset/public_data/IEEE_bigdata_RDD2020/test1.tar.gz
##### https://mycityreport.s3-ap-northeast-1.amazonaws.com/02_RoadDamageDataset/public_data/IEEE_bigdata_RDD2020/test2.tar.gz
