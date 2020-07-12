# Roads-and-Building-Segmentation
A repository for CNN based binary and semantic segmentation models for the task of segmenting roads and buildings from aerial images

# Execution
All the codes have been run on Google Colab. No additional Libraries are necessary.<br/>
The codes are coded in the python 3.x version

# Code

In this repository there are 3 files containing the network.<br/>

The first file is the jupyter notebook Deep_Learning_FCN.ipynb. This notebook details the [FCN-32](https://arxiv.org/pdf/1411.4038.pdf) model's configuration and also contains the training loop and test statistics generation. This file has been developed for the task of training and testing the network. For the purpose of deployment, a python file with the model architecture and a state dictionary import command can be used.<br/>

The second file is the jupyter notebook Deep_Learning_UNet.ipynb. This notebook details the [U-Net](https://arxiv.org/pdf/1505.04597.pdf)'s configuration and also contains the training loop and test statistics generation. This file has been developed for the task of training and testing the network. For the purpose of deployment, a python file with the model architecture and a state dictionary import command can be used.<br/>

The third file is the python file WebScrape.py. This file can be used to download the images from the Massachusetts Roads and Buildings Dataset hosted by the University of Toronto. The links for the train, test and validation datasets need to be changed for the roads and buildings dataset and the file can be run to download the data.
```
python WebScrape.py
```

# Dataset

The Dataset used for the Semantic Segmentation task is detailed in this [paper](https://arxiv.org/pdf/1707.06879.pdf)<br/>

Additional Datasets for Binary and Semantic segmentation are given below:<br/>
1) [Massachusetts Roads Dataset](https://www.cs.toronto.edu/~vmnih/data/) (Binary)
2) [Massachusetts Buildings Dataset](https://www.cs.toronto.edu/~vmnih/data/) (Binary)
3) [iSAID Dataset](https://captain-whu.github.io/iSAID/dataset.html) (Semantic and Instance). Link for the [Devkit](https://github.com/CAPTAIN-WHU/iSAID_Devkit)

For the two Massachusetts Datasets, the WebScrape.py can be used to extract the images into a folder

# Citation
1) Kaiser, Pascal, Jan Dirk Wegner, Aurélien Lucchi, Martin Jaggi, Thomas Hofmann and Konrad Schindler. “[Learning aerial Image segmentation from online maps.](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7987710)” IEEE Transactions on Geoscience and Remote Sensing 55 (2017): 6054-6068.
2) Ronneberger, Olaf, Philipp Fischer and Thomas Brox. “[U-Net: Convolutional networks for biomedical image segmentation.](https://arxiv.org/pdf/1505.04597.pdf)” MICCAI (2015).
3) Long, Jonathan, Evan Shelhamer and Trevor Darrell. “[Fully convolutional networks for semantic segmentation.](https://arxiv.org/pdf/1411.4038.pdf)” 2015 IEEE Conference on Computer Vision and Pattern Recognition (CVPR) (2015): 3431-3440.
4) Hinton, Geoffrey E. and Volodymyr Mnih. “[Machine learning for aerial image labeling.](http://www.cs.toronto.edu/~vmnih/docs/Mnih_Volodymyr_PhD_Thesis.pdf)” (2013).
5) Zamir, Syed Waqas, Aditya Arora, Akshita Gupta, Salman H. Khan, Guolei Sun, Fahad Shahbaz Khan, Fan Zhu, Ling Shao, Gui-Song Xia and Xiang Bai. “[iSAID: A large-scale dataset for instance segmentation in aerial images.](https://arxiv.org/pdf/1905.12886.pdf)” ArXiv abs/1905.12886 (2019):
