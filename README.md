# Generative Adversarial Network (GAN) based Image Compression

### Introduction
This project aims at creating an AI model to compress images while retaining as much quality as possible. The implementation is done (from scratch) using Tensorflow.
A GAN was created and trained on various kinds of images (from CIFAR, etc.). The trained model then is able to compress images belonging to three categories:
	1. Airplane
	2. Automobile
	3. Flower
Performance of the model was measured using several schemes that are usually used to compare two images. The difference between the original and compressed images were measured using:
	1. Mean Squared Error (MSE)
	2. Multiscale SSIM (MS-SSIM)
	3. Peak Signal to Noise Ratio (PSNR)
	4. L1 distance
	
	
### File Information
A short discription of the various files that are present in the repository is as follows:
Airplane_model.py:
	Contains the code to train model that is used to compress images of type 'Airplane'
Automobile_model.py:
	Contains the code to train model that is used to compress images of type 'Automobile'
Flower_model.py:
	Contains the code to train model that is used to compress images of type 'Flower'
compare_images.py:
	This file contains code to compare the original and compressed images
compress.py:
	This file integrates all the three models and compresses images based on the image type
convert_images.py:
	This file contains code that was used to convert the high resolution images in the Flower dataset to lower resolution so that it can be used to train the model (training on high resolution images was not computationally feasible)
data_extract.py:
	This file contains code to convert the images in the datasets into arrays that is then used totrain the model
stride.ai_project_proposal.pdf:
	This file contains the initial proposal for this project
team18_presentation.pdf:
	This file contains a short presentation on the project
team18_report.pdf:
	This file contains the project report
