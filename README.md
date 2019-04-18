# A Baseline System For CCKS-2019-IPRE

## Introduction
We provide a baseline system based on convolutional neural network with selective attention.

## Getting Started
### Environment Requirements
python 3.6

numpy

tensorflow 1.12.0

### Step 1: Download data
Please download the data from [the competition website](https://biendata.com/competition/ccks_2019_ipre/data/), then unzip files and put them in ./data/ folder.

### Step 2: Train the model
You can use the following command to train models for Sent-Track or Bag-Track:
```linux
python baseline.py --nopre_embed -nobag 
python baseline.py --nopre_embed --bag
```
The model will be stored in ./model/ floder. We also provide large scale unmarked corpus for train word vectors or language mdoels.
### Step 3: Test the model
You can use the following command to test models for Sent-Track or Bag-Track:
```linux
python baseline.py --mode test --nobag 
python baseline.py --mode test --bag
```
Predicted results will be stored in result_sent.txt or result_bag.txt
## Evaluation
We use f1 score as the basic evaluation metric to measure the performance of systems. In our baseline system, we get 0.22 in Sent-track and 0.31 in Bag-Track.
## References
* Lin Y, Shen S, Liu Z, et al. Neural relation extraction with selective attention over instances[C]//Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers). 2016, 1: 2124-2133.
