# BUS-BRA: A breast ultrasound dataset with BI-RADS categories

We introduce a breast ultrasound (BUS) dataset containing images of 1,064 patients that underwent routinary breast studies. The BUS dataset contains biopsy-proven tumor cases and BI-RADS annotations in categories 2, 3, 4, and 5. In addition, the dataset also contains ground truth delineations that divide the BUS images into tumoral and normal regions. Our dataset can be publicly accessed and downloaded through the open-access Zenodo repository (https://zenodo.org) under the collection named "BUS-BRA: A breast ultrasound dataset with BI-RADS categories" (https://doi.org/10.5281/zenodo.7730709), with the condition that any research originating from using the BUS-BRA dataset needs to cite this paper:

Wilfrido Gómez-Flores, Maria Julia Gregorio-Calas, and Wagner Coelho de Albuquerque Pereira, "A Breast Ultrasound Dataset with BI-RADS Categories for Benchmarking Computer-aided Diagnosis Systems," Medical Physics, 2023. (In revision)

Here, we provide the source codes to replicate the experiments in the article through two frameworks developed in Matlab 2022b:

1. Segmentation: It contains the functions for semantic segmentation of BUS images using the DeepLabV3+ model with ResNet18 and ResNet50 back-bone networks for feature extraction.
2. Classification:  It contains the functions for classifying BUS images into ways: 1) pathology classes in benign and malignant cases and 2) BI-RADS categories 2 to 5. The ResNet18 and ResNet50 deep networks are used for feature extraction.

The BUS-BRA dataset should first be downloaded and decompressed in the root directory. Then run the RUNME.m file inside the Classification and Segmentation folders to reproduce the experiments using 5-fold cross-validation.

![picture alt](https://github.com/wgomezf/BUS-BRA/blob/main/directory.png "Directory")
