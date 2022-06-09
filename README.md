# HybridMSSN-Model

* HybridMSSN Model for Hyperspectral Image Classification

**Description**
======

* The HybridMSSN model contains:
    * Three 3D-CNNs, 
    * One 2D-CNN, and 
    * Five Spinal Fully Connected Networks (SFCNs). 

* 3D-CNNs are used for joint spatial-spectral features learning from the input data.
* The 2D-CNN extracts more abstract level spatial representation from the features obtained from the last 3D-CNN.
* Multi Scale Feature learning strategy is employed to achieve the abstraction of image data at various scales.
* Spinal Fully Connected Networks (SFCNs) helps in improving the accuracy.
* We have used Google colab pro platform to run this code and generate the results.

# Datasets 

* Datasets can be downloaded from the official website of the Computational Intelligence Group of the University of the Basque Country (UPV/EHU) [https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes]


# Prerequisites

*  Tensorflow 2.8.0
*  Keras 2.8.0
*  Matplotlib
*  Numpy
*  Scipy
*  Sklearn

# Instructions to use this code

* Import Hybrid_MS_SpinalNet.ipynb file to your Google colab platform. We have used a GPU and a High RAM provided with Google colab pro subscription for simulating the results. 
* Upload the dataset and the correrponding groundtruth.
* Set the dataset, name variables to 'IP' for investigating on Indian Pines dataset. Similarly set 'PU' for Pavia University and 'SA' for Salinas dataset.
*  test_ratio denotes testing ratio. windowsize is used to select the size of 3D image patches.
* Run the individual code cells and observe the output.
* Classification report containing Test loss, Test accuracy, Kappa accuracy, Overall accuracy, Training time and Testing time will be saved in text file. We have named this file as 'classification_report.txt' in our code. You can give your own name.



