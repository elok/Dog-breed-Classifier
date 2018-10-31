[//]: # (Image Reference)

[image1]: ./notebook_images/sample_dog_result.png "Sample Output"
[image2]: ./notebook_images/vgg16_architecture.png "VGG-16 Architecture"

# Dog-breed Classifier

## Project Overview

It's the Convolutional Neural Network(CNN) project in the Deep Learning Nanodegree program of Udacity. I learned how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images. Given an image of a dog, my algorithm identifies an estimate of the dog's breed. If supplied an image of a human, the code identifies the resembling dog breed.

![Sample Output][image1]

## Project Instruction

### Instructions

1. Clone the repository and navigate to the downloaded floder.
	```	
		git clone https://github.com/choonghee-lee/Dog-breed-Classifier.git
		cd Dog-breed-Classifier
	```
2. Open the `Dog-breed Classifier_EN.ipynb`(English Version) or `Dog-breed Classifier_KR.ipynb` (Korean Version) file. Of course you can find HTML version of the two files.
	```
		jupyter notebook Dog-breed Classifier_EN.ipynb
		jupyter notebook Dog-breed Classifier_KR.ipynb
	```
3. Read and follow the instructions! This repository doesn't include any dataset you need. You can check out the notebook to download them.

 
## Project Information

### Contents

It's the contents of Korean Version file. The English one has similar contents:

- Intro
- Step 0: Import Datasets
- Step 1: Detect Humans
- Step 2: Detect Dog
- Step 3: Create a CNN to Classify Dog Breeds (from Scratch)
- Step 4: Create a CNN to Classify Dog Breeds (using Transfer Learning)
- Step 5: Write Your Algorithm
- Step 6: Test Your Algorithm

### Main CNN Model
I had tried to imitate VGG-16 in the step 3 and I used VGG-16 for the transfer learning in step 4. Here is the architecture of VGG-16:

![VGG-16 Architecture][image2]

### Libraries

The list below represents main libraries and its objects for the project.
- [PyTorch](https://pytorch.org/) (Convolutional Neural Network)
- [OpenCV](https://opencv.org/) (Human Face Detection)
- [Matplotlib](https://matplotlib.org/) (Plot Images)
- [Numpy](http://www.numpy.org/) (^^)

### Accelerating the Training Proecess

In the training step in the Step 3 and 4, it is taking too long to run so you will need to either reduce the complexity of the VGG-16 architecture or switch to running the code on a GPU.

#### Amazon Web Services

You can use Amazon Web Services to launch an EC2 GPU instance. (This costs money!)