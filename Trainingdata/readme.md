## Content-Aware Convolutional Neural Network for In-loop Filtering in High Efficiency Video Coding


### Brief Intro
This folder contains the materials for single CNN model training data generation in our paper.
As mentioned in our paper, we use BSDS-500 dataset for illustration.
Notes: The matlab code for generating training samples will be provided soon. 

### Detail
- generate_single_train.m: 80% of the dataset are used for training data generation. 
- generate_single_test.m: the remaining images for validation data. 
- store2hdf5.m: zip the data and store the them into .h5 format. 
- The folder 'Label' contains uncompressed BSDS500 dataset in .bmp format.
- The folder 'qp**' contains HEVC-compressed BSDS500 dataset in .bmp format, where ** denotes the QP value.
- Download link: [here](https://drive.google.com/file/d/15DRAOnyFIHcq-yGtxpbpwDxfMPWaWLTU/view?usp=sharing)

### Test
- Platform: MATLAB
- OS info: Win10 HomeBasic 64bit && 16G Memory
- Version: MATLAB 2017a

### Tips
- Modify the parameters to adapt your tasks when generating data.

### Reference
- C. Jia, S. Wang, X. Zhang, S. Wang, J. Liu, S. Pu and S. Ma, “Content-Aware Convolutional Neural Network for In-loop Filtering in High Efficiency Video Coding,” IEEE Trans. on Image Processing, 2019.
- Arbelaez, Pablo, et al. "Contour detection and hierarchical image segmentation." IEEE Transactions on Pattern Analysis and Machine Intelligence 33.5 (2011): 898-916.

### Author
- cmjia@pku.edu.cn

### License
- GPL v3  
