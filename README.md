# Multi-class-skin-cancer-classification
# Multi-class-skin-cancer-classification
The project aims at the fusion of segmentation and classification models for efficient classification of multi-class skin cancer
The skin cancer classification is done in a two step method.
Initially, segmentation is performed using spatial attention-guided UNet on the PH2/ISIC-2017/ISIC-2018 dataset and the weights are saved in the folder. The weights folder is not uploaded here due to size constraint.
EfiicientNet B1 model is used for classification. 
Multi-scale fusion property is used in this case for efficient classification of skin cancer.
In multi-scale fusion principle. The segmented weights, are used to extract the skin lesion and then image features are extracted form segmented images by EfficientNet B1 for classification on the ISIC- 2019/2018 dataset. These features are called local features. The global features from original images of the ISIC- 2019/2018 dataset are extracted using the EfficientNet B1 model. The local and global features are concatenated before the dense layers. The dense layers use the combined features for skin cancer classification.
The proposed methodology can also be extended to the binary classification on the ISIC- 2017/20 datasets.
The proposed methodology can be extended to other medical images for efficient segmentation and classification.
