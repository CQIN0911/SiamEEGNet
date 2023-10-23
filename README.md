# SiamEEGNet
This repository is the official implementation of 'SiamEEGNet: Siamese Neural Network-Based EEG Decoding for Drowsiness Detection'.

## Requirements
### Step 1.
To install requirements:
```
conda env create -f /path/to/SiamEEGNet_env.yml
conda activate SiamEEGNet_env
```
### Step 2.
Create a new empty folder 'data' in this folder. Download datasets and put them to the folder 'data'.

## Dataset
- Lane-keeping driving dataset task: https://figshare.com/articles/dataset/Multi-channel_EEG_recordings_during_a_sustained-attention_driving_task/6427334
- The sessions included in the experiment are shown in the selected_session_list.txt

## Training and inference
Train SiamEEGNet with within-subject training scheme
```
python train_within_subject.py
```
Train SiamEEGNet with cross-subject training scheme
```
python cross_within_subject.py
```
Inference using existing models
```
python inference.py --model_path model/
```
