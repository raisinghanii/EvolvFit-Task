# EvolvFit-Task

Please go to the link https://drive.google.com/file/d/1i4U7lfbK02Mh9sFHDlyvgkqIcrLl8vUd/view?usp=sharing for demo video.

First off to run the task you may need the weights. download it from https://drive.google.com/drive/folders/1uJ1A3CwsDU2mc1s85CloT7-hU2j699OC?usp=sharing

# To run or see the output go through livedetection file.


The Dataset is not a good one and very small due to which I was not able to train a good model

Dataset contained images like:
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/bhuvneshwar_kumar/c965e47869.jpg)
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/jasprit_bumrah/2751420e7e.jpg)
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/mohammed_shami/fdae0c1962.jpg)
![alt text](https://github.com/raisinghanii/EvolvFit-Task/blob/master/images/ravindra_jadeja/e96843617c.jpg)

And also contained photo of one cricketer in another cricketer's directory.


## First Step: Finding Faces and Arranging into train and validation/testing set:

To see this please go through foldering.ipynb

Here I've cropped the faces for training, discarding the useless information as to train the model better:

![image](https://user-images.githubusercontent.com/46864533/118835703-dde6af00-b8e0-11eb-81e6-2a30d9b36b15.png)

![image](https://user-images.githubusercontent.com/46864533/118835781-edfe8e80-b8e0-11eb-80d6-380dd06a061d.png)

![image](https://user-images.githubusercontent.com/46864533/118835856-fce54100-b8e0-11eb-9c74-d17fca0a4e37.png)

![image](https://user-images.githubusercontent.com/46864533/118835913-0a023000-b8e1-11eb-964d-446148e8bbea.png)

![image](https://user-images.githubusercontent.com/46864533/118836144-3d44bf00-b8e1-11eb-9dd3-978f31fce17f.png)


The above was done using haarcascade in OpenCV.



