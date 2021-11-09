# Object_detection-fish_and_path_prediction
# Steps:

1.Prepare your dataset and label them in YOLO format using 'LabelImg'. Once done, zip all the images and their corresponding label files as images.zip.

2.Create a folder named yolov3 on Google Driveand upload the images.zip file inside it. The directory structure should look something like the following:
```bash
yolov3
|__images.zip
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
You can also download the same file from my github repository 
and change the file location in the code.
```bash
net = cv2.dnn.readNetFromDarknet("/Users/anubhav/Desktop/yolov3_custom.cfg",
                                 "/Users/anubhav/Desktop/yolov3-obj_30000.weights")
```

6.Downloaded the video files and save them inside the repository you had cloned on your local machine.


7.Open the Obj_detection_and_path_prediction.ipynb file inside the repository and edit with the name of the video file you want to the test.
```bash
cap = cv2.VideoCapture('/Users/anubhav/Desktop/fish_clip_s.mp4')
```




![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/76263415/140932458-72276e58-e8ab-427c-8140-b0f96945d4c4.gif)
# Path pediction plot using Forecasting Model(SARMIAX)
![image](https://user-images.githubusercontent.com/76263415/140932184-85c7f03d-7432-4e93-9945-c1e6302d1687.png)





