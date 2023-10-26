# Object-Detect-Guru
Real time Object Detection and Segmentation

This is an implementation of Mask R-CNN on Python 3, Keras, and TensorFlow. The model generates bounding boxes and segmentation masks for each instance of an object in the image. It's based on Feature Pyramid Network (FPN) and a ResNet101 backbone.

## The repository includes:

Source code of Mask R-CNN built on FPN and ResNet101.
Training code for MS COCO
Pre-trained weights for MS COCO
Jupyter notebooks to visualize the detection pipeline at every step
ParallelModel class for multi-GPU training
Evaluation on MS COCO metrics (AP)
Example of training on your own dataset
The code is documented and designed to be easy to extend. If you use it in your research, please consider citing this repository (bibtex below). If you work on 3D vision, you might find our recently released Matterport3D dataset useful as well. This dataset was created from 3D-reconstructed spaces captured by our customers who agreed to make them publicly available for academic use.

## Requirements
Python 3.4, TensorFlow 1.3, Keras 2.0.8 and other common packages listed in requirements.txt.

## MS COCO Requirements:
To train or test on MS COCO, you'll also need:

## pycocotools (installation instructions below)
MS COCO Dataset
Download the 5K minival and the 35K validation-minus-minival subsets. More details in the original Faster R-CNN implementation.
If you use Docker, the code has been verified to work on this Docker container.

## Installation
Clone this repository

## Install dependencies

pip3 install -r requirements.txt
Run setup from the repository root directory

python3 setup.py install
Download pre-trained COCO weights (mask_rcnn_coco.h5) from the releases page.

## (Optional) 

To train or test on MS COCO install pycocotools from one of these repos. They are forks of the original pycocotools with fixes for Python3 and Windows (the official repo doesn't seem to be active anymore).

Linux: https://github.com/waleedka/coco
Windows: https://github.com/philferriere/cocoapi. You must have the Visual C++ 2015 build tools on your path (see the repo for additional details)
