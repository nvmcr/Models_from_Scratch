# Models_from_Scratch
## Goal
In this problem we consider building classifiers for a 15-way fruit classification task. The dataset we
consider is comprised of a set of 256 × 256 × 3 (256 × 256 pixels and 3 color channels) images of various
types of fruit. The objective is to use the provided data to come up with a classifier that achieves high
accuracy on a test set.
## Dataset
You can get the datasets from this google drive: [Link](https://drive.google.com/drive/folders/1kJb8Hs7s8txeEGsOfbB-f5gYAzMVQnph?usp=sharing). It is one zipped file called datasets.zip containing both the train and validation data, and that is about 1.8GB big. After this data is uncompressed, it creates a directory called ./datasets that contains the .pkl files that, together, are about 8.6GB big. The training set contains n = 9, 876 image samples while the validation set contains n = 2, 116 samples. In each dataset, we provide the following:
* images: the raw RGB images
* feats: m = 15 dimensional real-valued condensed representations of each image (these were precomputed by using a pretrained neural network for feature extraction followed by PCA to reduce the
dimensionality down to m = 15)
* labels: an integer value between 0 and 14 giving the class label. The integer to class mapping is
provided below in the variable idx to class. 
The test set will include both a set of images and a 15-dimensional featurization of those images in exactly the same form as the features that were given for the train and validation set. It is available in the same link. 
## Scratch Model
Models like Logistc Regression, Decision Trees, Random Forests and K-Nearest Neighbors are implemented from scratch in the notebook. Along with the scratch models, bunch of other models were also implemented. 
## Usage
For a quick glance, click on the `fruit_classification.ipynb` which has all the code and outputs with explanations. To reproduce follow the below usage steps:
1. Open your terminal
2. Clone the repoistory using `git clone git@github.com:nvmcr/Models_from_Scratch.git`.
3. This will create a repository with the name `Model_from_Scratch`.
4. Enter the present repo using `cd Model_from_Scratch/`.
5. Set up a new virtual environment with all necessary packages and dependencies using `conda env create -f environment.yml`
6. Activate the virtual environment with `conda activate ee-511`.
7. Open the notebook, explore and run.
8. You can deactivate the virtual environment later using `conda deactivate`
