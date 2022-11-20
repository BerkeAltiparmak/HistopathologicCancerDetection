# HistopathologicCancerDetection
A CNN model that identifies metastatic cancer in small image patches taken from larger digital pathology scans to compete at a Kaggle competition. 
Created to present it at the 3rd workshop of University of Toronto Machine Intelligence Student Team (UTMIST).

# UTMIST Workshop #3: Histopathologic Cancer Detection
Hello UTMIST community!

In this workshop, we will be building a model that will compete at a Histopathologic Cancer Detection Competition on Kaggle, which can be found here https://www.kaggle.com/competitions/histopathologic-cancer-detection.
As stated on their website, our algorithm will identify metastatic cancer in small image patches taken from larger digital pathology scans. The data for this competition is a slightly modified version of the PatchCamelyon (PCam) benchmark dataset. In this dataset, we are provided with a large number of small pathology images to classify. Files are named with an image id. The train_labels.csv file provides the ground truth for the images in the train folder. You are predicting the labels for the images in the test folder. A positive label indicates that the center 32x32px region of a patch contains at least one pixel of tumor tissue. Tumor tissue in the outer region of the patch does not influence the label. This outer region is provided to enable fully-convolutional models that do not use zero-padding, to ensure consistent behavior when applied to a whole-slide image.


Authors: Berke Altiparmak (altiparmak.berke@gmail.com), Lindy Zhai (lindy.zhai@mail.utoronto.ca)


References:
* https://www.kaggle.com/code/bonhart/pytorch-cnn-from-scratch for the model.
* https://www.kaggle.com/code/gomezp/complete-beginner-s-guide-eda-keras-lb-0-93 for data visualization.
