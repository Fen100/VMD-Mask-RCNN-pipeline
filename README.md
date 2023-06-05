# Mask R-CNN pipeline for detecting vessels on the VMD
This GitHub repository contains the pipeline for detecting and segmenting sand mining river vessels on the Vietnam Mekong Delta, using PlanetScope imagery and Mask R-CNN. The dimensions of these vessels were used to compose a sand budget for the Mekong river in the provinces of An Giang and Dong Thap, Vietnam.

## Contents
This repository includes:
* Source code of Mask R-CNN built on FPN and ResNet101
* Pre-trained weights for MS COCO
* A Jupyter notebook to run the VMD pipeline
* Zipped folder with Train and Validation datasets named 'Annotationdata'
* Zipped folder with Test dataset named 'test'

The train, validation and test datasets were annotated with VGG Image Annotator. The annotations are .json files.

## Dependencies
### Mask R-CNN requirements.txt
* numpy
* scipy
* Pillow
* cython
* matplotlib
* scikit-image==0.16.2
* tensorflow==1.15
* keras==2.2.5
* opencv-python
* h5py==2.10.0
* imgaug
* IPython[all]

These exact scikit-image, tensorflow, keras and h5py versions are required to work with the Mask R-CNN Matterport repository.

### Setup on a Windows PC
This is the set up that I used to run the model:
* Windows 10 64bit
* NVIDIA graphics card GeForce RTX 2070 Super
* Anaconda with Python 3.7.11
* CUDA 10.0
* CuDNN 7.6.5

This exact version of CUDA is required to work with the Mask R-CNN Matterport repository.
