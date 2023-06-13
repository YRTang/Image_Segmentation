# GI Tract Image Segmentation


## Dataset: 
* Link from Kaggle: https://www.kaggle.com/competitions/uw-madison-gi-tract-image-segmentation/data?select=train
* Link from project Google Drive:
train:
https://drive.google.com/drive/folders/19xLnW9qctKuz1dZLvKqhJnXw-odUMY6R?usp=share_link
label2:
https://drive.google.com/drive/folders/18LMCborta8nWo2R-Rl1KNWd4RvclT-2c?usp=share_link

## Instruction
### Step 1:
To run the sample.ipynb, run the following commands:

###'!pip install -q segmentation_models_pytorch'
###'!pip install -qU wandb'
###'!pip install -q scikit-learn==1.0'
###'!pip install colorama'


### Step2:
train.csv: original data information from Kaggle, containing image scans’ id, classes, and RLE segmentation array if provided.
train_data3.csv: contains the data from train.csv with extra information, which are image paths, mask paths, height, width, if it is empty, the fold number it resides.
train: contains original input images.
label2 folder: contains .npy mask images with three dimensions: (height, width, channel)


To run the sample.ipynb,
Download train_data3.csv, label2 folder, and train folder, also download “best_epoch-00.bin” which stores the best model summary
