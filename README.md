# Social-Distance-Monitoring-and-Face-Mask-Detection

datasets used 
https://drive.google.com/drive/folders/1ULdjQf7G5maksfmEjSUwUdfLCtm5IVQ0?usp=sharing
![image](https://user-images.githubusercontent.com/72460414/132217813-cf2215d9-cbc8-4b20-adf9-cfc9d7179dee.png)


Firstly, the dataset would be trained for classifying whether a face is masked or not. Hence, we need a diverse dataset that contains faces in various orientations and lighting conditions. The dataset should cover people of different ages and gender. Finding such wide range of pictures becomes a challenging task. Thus, numerous kinds of Augmentation would be applied. The dataset with various images of faces is taken as input and two augmentation techniques namely masked face augmentation and blurring augmentation are applied and the augmented images of the faces is obtained as the output. Then we give a video as an input to monitor social distancing and detect face masks. This video is converted as frames and read one by one. Then, to detect persons from the frames, we will be using YOLO (You Only Look Once), an effective real time object recognition algorithm that places bounded boxes around the detected persons. To detect the faces of the detected persons DSFD (Dual Shot Face Detector) would be used because it produces accurate results than any other face detection method.Then, DBSCAN (Density-based spatial clustering of applications with noise) clustering method would be used to detect the distance between detected persons. The colour of the bounded box differentiates safe (green-coloured box) and unsafe (red-coloured box) persons.


EXPERIMENTAL RESULTS

The experimental results obtained from each module are listed below.

MODULE 1: DATA AUGMENTATION

1.1MASKED FACE AUGMENTATION

![image](https://user-images.githubusercontent.com/72460414/132219202-8e2f5200-de1b-40cd-a439-943e5fea71ec.png)

A sample image for the masked face augmentation is shown on the right-hand side which can be compared with the original image shown on the left-hand side.
1.2 BLURRING AUGMENTATION

![image](https://user-images.githubusercontent.com/72460414/132219232-51b781bf-0b36-4b59-9b9f-920d5e2bde7e.png)

A sample image for the blurring augmentation is shown on the right-hand side which can be compared with the original image shown on the left-hand side.

MODULE 2: FACE MASK CLASSIFIER


TESTING THE FACE MASK CLASSIFIER ON AN IMAGE

![image](https://user-images.githubusercontent.com/72460414/132218902-340e9a03-4207-42c7-a9f1-f4a1dc15e710.png)
![image](https://user-images.githubusercontent.com/72460414/132218916-468f73de-3d8a-46f7-91b0-eb7e131415ef.png)

the red box around the face indicates no mask on the face while the green mask around the face indicates masked face.

MODULE 3 - SOCIAL DISTANCE MONITORING

![image](https://user-images.githubusercontent.com/72460414/132218777-6f05dc56-8f93-44c0-b91a-4224e029fe14.png)

   Input Video – sample image

![image](https://user-images.githubusercontent.com/72460414/132218700-eec18cae-50bc-4b73-b54f-c6a3f444a139.png)

  Output Video - sample image


Team members:-

Mithun Raam M

NarenTP

Sanjay Chinni Karthick V
