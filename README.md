# Social-Distance-Monitoring-and-Face-Mask-Detection

datasets used 
https://drive.google.com/drive/folders/1ULdjQf7G5maksfmEjSUwUdfLCtm5IVQ0?usp=sharing
![image](https://user-images.githubusercontent.com/72460414/132217813-cf2215d9-cbc8-4b20-adf9-cfc9d7179dee.png)


Firstly, the dataset would be trained for classifying whether a face is masked or not. Hence, we need a diverse dataset that contains faces in various orientations and lighting conditions. The dataset should cover people of different ages and gender. Finding such wide range of pictures becomes a challenging task. Thus, numerous kinds of Augmentation would be applied. The dataset with various images of faces is taken as input and two augmentation techniques namely masked face augmentation and blurring augmentation are applied and the augmented images of the faces is obtained as the output. Then we give a video as an input to monitor social distancing and detect face masks. This video is converted as frames and read one by one. Then, to detect persons from the frames, we will be using YOLO (You Only Look Once), an effective real time object recognition algorithm that places bounded boxes around the detected persons. To detect the faces of the detected persons DSFD (Dual Shot Face Detector) would be used because it produces accurate results than any other face detection method.Then, DBSCAN (Density-based spatial clustering of applications with noise) clustering method would be used to detect the distance between detected persons. The colour of the bounded box differentiates safe (green-coloured box) and unsafe (red-coloured box) persons.

team members:-
Mithun Raam M
NarenTP
Sanjay Chinni Karthick V
