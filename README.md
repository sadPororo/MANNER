# MANNER (Multi-view Attention Network for Noise ERasement)

This is a Pytorch implementation of MANNER: Multi-view Attention Network for Noise ERasement. MANNER is a deep learning model for speech enhancement in time-domain. MANNER consists of encoder-decoder based on U-net. Each encoder and decoder contains Up/Down conv, Residual Conformer block, and Multi-view Attention block. MANNER representing full information of the signal efficiently addresses channel and long sequential features. Experimental results on the VoiceBank-DEMAND dataset suggest that MANNER achieves state-of-the-art performance. In addition, among time-domain models, MANNER shows the efficient results in terms of inference speed and memory usage.


# Installation & Enviornment

# Prepare for usage

## 1. Prepare dataset

We use VoiceBank-DEMAND (Valentini) dataset consisting 28 speakers for training MANNER. 

- The dataset can be downloaded [here](https://datashare.ed.ac.uk/handle/10283/2791).

## 2. Downsample

The sample rate of the dataset is 48kHz.

For a fair comparison we downsample the audio files from 48kHz to 16kHz.

- To downsample the audio, run the following code and edit the directorys.

  ```
  python downsampling.py
  ```
  
- In the downsampleing.py script, you should change the contents as follows.
  
  ```
  downsample_rate = 16000
  clean_train_path = 'The original clean trainset path'
  noisy_train_path = 'The original noisy trainset path'
  clean_test_path = 'The original clean testset path'
  noisy_test_path = 'The original noisy testset path'
  resample_path = 'Resampled path'
  ```
  
## 3. Make data path files





# How to use

## 1. Train

## 2. evaluation

## 3. Pretrained weights

## 4. Configuration

## 5. Logging

# Citation

# License
