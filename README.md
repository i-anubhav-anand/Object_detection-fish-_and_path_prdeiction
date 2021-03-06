# Object detection and path prediction using forecasting algorithm

# Introduction:

1.Trained an object detection model using Darknet to identify the subject.

2.Tracked the position of the object and predicted its path based on the previous points.


# Steps:

1.Prepare your dataset and label them in YOLO format using 'LabelImg'. Once done, zip all the images and their corresponding label files as images.zip.

2.Create a folder named yolov3 on Google Driveand upload the images.zip file inside it. The directory structure should look something like the following:
```bash

fish_images_annotated_yolo_formal.zip
   |__ *.jpg (all image files)
   |__ *.txt (all annotation files)
```
3.Clone the repository and upload the train_fish_custom_dataset_yolo.ipynb
 notebook on Google Colab.

4.Run the cells one-by-one by following instructions as stated in the notebook. For detailed explanation, refer the following document.

5.Once the training is completed, download the following files from the yolov3 folder saved on Google Drive, onto your local machine.
```bash
yolov3_training_last.weights
yolov3_custom.cfg
classes.txt
```
(You can also download the same file from my github repository 
and change the file location in the code.

You can download trained weights from here
https://www.dropbox.com/s/gmw2774nrsw7ovk/yolov3-obj_30000.weights?dl=0)
```bash
net = cv2.dnn.readNetFromDarknet("/Users/anubhav/Desktop/yolov3_custom.cfg",
                                 "/Users/anubhav/Desktop/yolov3-obj_30000.weights")
```

6.Downloaded the video files and save them inside the repository you had cloned on your local machine.


7.Open the Obj_detection_and_path_prediction.ipynb file inside the repository and edit with the name of the video file you want to the test.
```bash
cap = cv2.VideoCapture('/Users/anubhav/Desktop/fish_clip_s.mp4')
```


https://user-images.githubusercontent.com/76263415/143421625-6b64d3af-49fb-4741-afe0-283ee35c199e.mp4





# Path pediction plot using AR(Autoregressive) Forecasting Model

Prediction of Y-cordinate of Centroid<br>
<img width="334" alt="image" src="https://user-images.githubusercontent.com/76263415/143440657-cdf9b763-c048-4dab-97b0-25e0287d7b3e.png">

Prediction of X-cordinate of Centroid<br>
<img width="325" alt="image" src="https://user-images.githubusercontent.com/76263415/143440706-4f382e9d-d6ae-427d-b016-15e62d5e4462.png">



# Path pediction plot using Forecasting Model(VAR)
<img width="567" alt="image" src="https://user-images.githubusercontent.com/76263415/143420834-d7a02244-5656-451f-a420-6145d7f00ea8.png">




