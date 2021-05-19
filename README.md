# EvolvFit-Task

Please go to the link https://drive.google.com/file/d/1i4U7lfbK02Mh9sFHDlyvgkqIcrLl8vUd/view?usp=sharing for demo video.

First off to run the task you may need the weights. download it from https://drive.google.com/drive/folders/1uJ1A3CwsDU2mc1s85CloT7-hU2j699OC?usp=sharing

## To run or see the output go through livedetection file.


The Dataset is not a good one and very small due to which I was not able to train a good model

Dataset contained images like:
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/bhuvneshwar_kumar/c965e47869.jpg)
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/jasprit_bumrah/2751420e7e.jpg)
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/mohammed_shami/fdae0c1962.jpg)
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/ravindra_jadeja/e96843617c.jpg)

And also contained photo of one cricketer in another cricketer's directory.


## Step 1: Finding Faces and Arranging into train and validation/testing set:

To see this please go through foldering.ipynb

Here I've cropped the faces for training, discarding the useless information as to train the model better:

![image](https://user-images.githubusercontent.com/46864533/118836323-5e0d1480-b8e1-11eb-865e-f09ccf392b1d.png)

![image](https://user-images.githubusercontent.com/46864533/118835781-edfe8e80-b8e0-11eb-80d6-380dd06a061d.png)

![image](https://user-images.githubusercontent.com/46864533/118835856-fce54100-b8e0-11eb-9c74-d17fca0a4e37.png)

![image](https://user-images.githubusercontent.com/46864533/118835913-0a023000-b8e1-11eb-964d-446148e8bbea.png)

![image](https://user-images.githubusercontent.com/46864533/118836144-3d44bf00-b8e1-11eb-9dd3-978f31fce17f.png)


The above was done using haarcascade in OpenCV.

## Step 2: Trying different models and saving the model:

First I have created ImageDataGenerator and done Image Augmentation(which means applying various filters and disturbance or flips on the image) as to help the model learn even in difficult situations and distorted or hard test cases.see the output below:

![image](https://user-images.githubusercontent.com/46864533/118836929-f86d5800-b8e1-11eb-9eee-86a3fe2632ac.png)


Then I've used various pretrained state of the art models to get good results.

I have tried MobilenetV2, InceptionV3, VGG16 and ResNet.

### You can find the code of this in task file and their copy where I was just playing and trying different algos.

## There is no specific accuracy, you can go through the notebook and see that in most cases training accuracy is around 90% but validation accuracy is around 40% which means the model is overfitting due to small and bad data.

There was a VGG16 model which was giving comparatively good results which I have saved and used further.

## Step 3: Creating Live Detection module and testing.

You can refer the video for live detection.

This was done using OpenCv and HaarCascade to identify faces and pass them into the model.
The model is not performing good though.
