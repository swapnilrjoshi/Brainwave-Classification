# Brainwave-Classification
This repo provides two Convolutional Neural Networks(CNN) based on VGG architecture to achieve end-to-end brainwave classification. Simple 1D CNN directly accepts processed brainwave while for more elaborate 2D CNN brainwave is first passed through a filter-bank of 16 filters to create a 2D image. The experiments are performed using synthesized Local Field Potential(LFP) brainwave data with different noise levels. The networks achieve an accuracy of 75.19% and 76.03% resp. for a dataset with -11.94dB average SNR.  
# Usage
1. Create data using data_set.m from data folder.
2. Create 2D images using preprocessing
3. Change filenames in data_loading.py
4. Use CNN1D_model.py and CNN2D_model.py to train the networks using train and test data or use cross_validation.py to train using 5-fold    cross-validation
