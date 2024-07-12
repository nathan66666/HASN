# HASN

## Overview framework
![hasn](figs/HASN.png)

## Dependencies and Installation
```
## git clone this repository
git clone https://github.com/nathan66666/HASN.git
cd HASN

# create an environment with python=3.9
conda create -n hasn python=3.9.17
conda activate hasn
pip install -r requirements.txt
```

## Quick Inference
#### Step 1: Download the pretrained models
You can put the  HASN model  in the `experiments`.
#### Step 2: Prepare testing data
You can put the testing images in the `datasets/test_datasets`.

#### Step 3: Running testing command
```
python basicsr/test.py -opt options/test/test_HASN.yml
```
## Train 

#### Step1: Prepare training data
- Download the training data from (https://github.com/XPixelGroup/BasicSR/blob/master/docs/DatasetPreparation.md)

#### Step2: Training for HASN
```
CUDA_VISIBLE_DEVICES=0 python basicsr/train.py -opt /options/train/HASN/train_HASN.yml
```


## Acknowledgments
This project is based on [BasicSR](https://github.com/XPixelGroup/BasicSR).


## 📧 Contact
If you have any questions, please feel free to contact: `xyan_lei@163.com`
