# Lung-lobe-segmentation
Some resources (papers, websites, codes, books, videos, etc) for lung lobe segmentation using deep learning.

## Some websites for semantic segmentation
https://github.com/mrgloom/awesome-semantic-segmentation 

## Papers for lung lobe segmentation
Papers uploaded to arxiv.org will be linked to the pdf file, while others will be linked to the corresponding publisher website.

1. Tang, H., C. Zhang, and X.J.a.p.a. Xie, [Automatic Pulmonary Lobe Segmentation Using Deep Learning](https://arxiv.org/pdf/1903.09879.pdf). 2019.  
2. Tan, J., et al., [LGAN: Lung Segmentation in CT Scans Using Generative Adversarial Network](https://arxiv.org/pdf/1901.03473.pdf). 2019.  

3.Park, J., et al., [Fully Automated Lung Lobe Segmentation in Volumetric Chest CT with 3D U-Net: Validation with Intra- and Extra-Datasets. J Digit Imaging](https://www.ncbi.nlm.nih.gov/pubmed/31152273), 2019.   
4.Lee, H., et al., [Efficient 3D Fully Convolutional Networks for Pulmonary Lobe Segmentation in CT Images](https://arxiv.org/pdf/1909.07474.pdf). 2019.  
5.Gerard, S.E. and J.M. Reinhardt. [Pulmonary Lobe Segmentation Using A Sequence of Convolutional Neural Networks For Marginal Learning](https://ieeexplore.ieee.org/document/8759212). in 2019 IEEE 16th International Symposium on Biomedical Imaging (ISBI 2019). 2019. IEEE.] 
6.[Ferreira, F.T., et al. End-to-end supervised lung lobe segmentation. in 2018 International Joint Conference on Neural Networks (IJCNN). 2018. IEEE.](https://ieeexplore.ieee.org/document/8489677)  
7.[George, K., et al., Pathological pulmonary lobe segmentation from ct images using progressive holistically nested neural networks and random walker, in Deep Learning in Medical Image Analysis and Multimodal Learning for Clinical Decision Support. 2017, Springer. p. 195-203.](https://link.springer.com/chapter/10.1007/978-3-319-67558-9_23)  
8.[Milletari, F., N. Navab, and S.-A. Ahmadi. V-net: Fully convolutional neural networks for volumetric medical image segmentation. in 2016 Fourth International Conference on 3D Vision (3DV). 2016. IEEE.](https://arxiv.org/pdf/1606.04797.pdf)  
9.[Ronneberger, O., P. Fischer, and T. Brox. U-net: Convolutional networks for biomedical image segmentation. in International Conference on Medical image computing and computer-assisted intervention. 2015. Springer.](https://arxiv.org/pdf/1505.04597.pdf)  
10.[Wang, W., et al., Automated Segmentation of Pulmonary Lobes using Coordination-Guided Deep Neural Networks. 2019.]  (https://arxiv.org/pdf/1904.09106.pdf)

## Dataset

[Part of LUNA16](https://github.com/deep-voxel/automatic_pulmonary_lobe_segmentation_using_deep_learning) [The only public lung lobe annotations I found. There are 50 manual annotations for 3D CT scans selected from [LUNA16](https://luna16.grand-challenge.org/)]

[LTRC](https://ltrcpublic.com/) [The lung tissue research consortium DCC has **stopped** accepting new applications for specimens and/or data as of September 20, 2019. NHLBI is preparing to transfer all specimens and data to its BioLINCC repository. Information on how to request LTRC resources after September 20 is forthcoming.]

[LIDC-IDRI](https://wiki.cancerimagingarchive.net/display/Public/LIDC-IDRI)[Lung Image Database Consortium image collection **does not** provide lung lobe segmentation annotations]


## How to overcome GPU memory limitation
GPU memory limitation is an inevitable challenge for 3D medical image segmentation. Some methods have been proposed for this problem.

1. Down-sampling [Most papers will downsample input 3D images, this can sacrifice the performance]

2. 3D patches [Some papers use 3D patches cropped from the original 3D CT scans for training and testing]

3. Parallel(Multi-GPU) training 
  - Data parallism
  - Model parallism
  - Pipline
  

 
4. Dilated Convolution [increase receptive field]

## Softwares/tools used for medical image analysis and visualization
- 3D slicer
- MeVisLab
- ImageJ (Fuji)
- ITK-SNAP
- Radiant dicom viewer



