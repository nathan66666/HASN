# AECSR

## Overview framework
![acesr](figs/aecsr.png)

## Dependencies and Installation
```
## git clone this repository
git clone https://github.com/nathan66666/AECSR.git
cd AECSR

# create an environment with python=3.9
conda create -n acesr python=3.9.17
conda activate acesr
pip install -r requirements.txt
```

## Quick Inference
#### Step 1: Download the pretrained models
- Download the pretrained AECSR model from [GoogleDrive](https://drive.google.com/file/d/1MOTJWK1I_n9tV1KNNrc5JfExPTrDfsB8/view?usp=drive_link)
#### Step 2: Prepare testing data
You can put the testing images in the `datasets/test_datasets`.

#### Step 3: Running testing command
```
python basicsr/test.py -opt options/test/test_AECSR.yml
```
## Train 

#### Step1: Prepare training data
- Download the training data from (https://github.com/XPixelGroup/BasicSR/blob/master/docs/DatasetPreparation.md)

#### Step2: Training for AECSR
```
CUDA_VISIBLE_DEVICES=0 python basicsr/train.py -opt /options/train/AECSR/train_AECSR.yml
```


## Acknowledgments
This project is based on [BasicSR](https://github.com/XPixelGroup/BasicSR).


## 📧 Contact
If you have any questions, please feel free to contact: `xyan_lei@163.com`
