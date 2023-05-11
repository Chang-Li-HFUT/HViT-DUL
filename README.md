# HViT-DUL
Code for paper: EEG-based seizure prediction via hybrid vision transformer and data uncertainty learning

## About the paper
* Title: EEG-based seizure prediction via hybrid vision transformer and data uncertainty learning
* Authors: Zhiwei Deng, Chang Li, Rencheng Song, Xiang Liu, Ruobing Qian, Xun Chen
* Institution: Hefei University of Technology
* Published in: Engineering Applications of Artificial Intelligence
## Instructions
* Before running the code, please download the CHB-MIT and Kaggle dataset, unzip them and place them into the right directory. You can modify the path of the CHBMIT and Kaggle dataset directory in the_SETTINGS_CHBMIT.json_:"datadir" and _SETTINGS_Kaggle.json_:"datadir", respectively.
* "cachedir" is the path to save .hickle files. Each .hickle data file contains the EEG signals and consponding labels of a subject. There are 2 arrays in the file: **data** 
and **labels**. The shape of **data** for CHB-MIT is (128, 1, 1280, 22). The shape of **label** is (128,). 
* leave one out cross-validation is used.
* The CHB-MIT dataset can be found [here](https://physionet.org/content/chbmit/1.0.0/).
* The Kaggle dataset can be found [here]( https://www.kaggle.com/c/seizure-prediction/data).

## Requirements
+ Pyhton 3.7
+ pytorch (1.11.0 version)
+ hickle (5.0.2)
+ h5py (3.8.0)
+ mne (1.3.1)
+ scikit-learn (1.2.2)
+ scipy (1.10.1)
* If you have any questions, please contact zhiweideng@mail.hfut.edu.cn
