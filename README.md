# A Baseline System For CCKS-2019-IPRE

## Introduction
We provide a baseline system based on convolutional neural network with selective attention.

## Getting Started
### Environment Requirements
python 3.6

numpy

tensorflow 1.12.0

### Step 1:Download data
Please download the data from [the competition website](https://biendata.com/competition/ccks_2019_ipre/data/), then unzip files and put them in ./data/ folder.

### Step 2:Train the model
You can use the following command to train models for Sent-Track or Bag-Track:
```python
python baseline.py --bag
python baseline.py --nobag
```
## References
* Lin Y, Shen S, Liu Z, et al. Neural relation extraction with selective attention over instances[C]//Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers). 2016, 1: 2124-2133.
