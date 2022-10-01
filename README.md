# Face_Mask_Detection
Abstract

Severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2) pandemic is still continuously spreading all over the world. With the advent of the omicron variant ,the situation is still under speculation in many parts of the world.Different studies have shown that usage of masks is the most significant way to avoid spreading of the virus from one person to another through air.Hence, it becomes crucial for people in public areas to wear masks.In this paper,the model trained and tested helps to identify individuals who are wearing a mask properly or not.This could be done in a public place which can be monitored using cameras such as Closed-Circuit Television (CCTV) cameras .The model works on image processing and deep learning technologies. The model was trained on a real-world dataset and successfully tested using live video streaming. Improve the model's accuracy by experimenting with different variables, many people at varying distances and hyper characteristics and the frame's position has been determined. This study is beneficial in combating the spread of the virus and avoiding contact with the virus. The proposed model's superior performance makes it ideal for video surveillance systems.
Keywords : DeepLearning, Computer Vision, OpenCV, Tensorflow, Keras.

METHODOLOGY
The model proposed here is designed and modeled using python libraries namely Tensorflow, Keras and OpenCV. CNN identifies and categorises images based on previously learned properties. When getting and assessing the necessary features of graphical images in a multi-layered structure, it is particularly effective. Figures 1 through 3 depict the outline of the proposed approach for identifying facemasks. It describes the proposed system, which is entirely made up of picture acquisitions as illustrated in fig. 1. In fig. 2, a person wearing a facemask and not wearing a facemask, as well as a CNN architecture categorization, are used to collect data.
Fig.1:

Fig.2: 


Fig.3:  

For this we collected a database of images which consist of about 1376 images with 690 images containing people wearing face masks and 686 containing  people without masks. By developing the model and using these images we can predict whether a person is  wearing a mask or not using a web-cam.
1: Dataset will be augmented  to include more images for our training. In this step of data augmentation, we will rotate and flip each of the images in our dataset.
2: Visualization of total images in the data set  will be done.
3: We split our data into the training set which will contain the images on which the CNN model will be trained and the testset with the images on which our model will be tested. And then we will build our Sequential model with various layers such as Conv2D, MaxPooling2D, Flatten, Dropout and Dense.
4: We will fit images in the training set using Keras library.
5: We will be using the HaarFeature-basedCascadeClassifiers for detecting the features of the face. This cascade classifier is designed by OpenCV to detect the frontalface by training thousands of images.
6: In the last step, we will use the OpenCV library to run an infinite loop to use our web camera in which we detect the face using the CascadeClassifier.The resulting model will predict the possibility of each of the two classes ([without mask, and  with mask]). Based on which probability will be higher, the label will be chosen and displayed around faces.

