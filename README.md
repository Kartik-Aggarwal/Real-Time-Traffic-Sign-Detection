# Real-Time-Traffic-Sign-Detection

## Abstract

Detection and classification of traffic signs in real time. ROI is enclosed in a bounding box and associated label is displayed on top of it. Yolov5-small object detection algorithm is used. Trained for 800 epochs on 3000 images manually labeled for 61 different classes. Achieved 91.75% mAP@0.5 and real time speed of 45 fps on GeForce MX 250

## Directions to run the code
1. Unzip the whole repository and make it your current directory
2. Find *Models.zip* inside the current directory and unzip it 
3. Install all the required dependencies using teh requirments.txt file
    * if you are using windows machine
    * **Type** - `pip install -r requirements.txt`
    * Or if you are using anaconda prompt
    * **Type** - `conda install --file requirements.txt`
4. Go to the directory named *Codes* using `cd Codes`
5. Before running the next command, put the image/video file, in which you want to detect traffic signs  in the directory named *Test*
    * **Type** - `python detect.py --source ../Test/{name of your file}`
    * For example if image name is test.jpg then type ` python detect.py -- source ../Test/test.jpg`
6. For running on live camera feed 
    * **Type** - `python detect.py --source 0`
7. Outputs are saved in *Results folder*

## Directory structure
**Real-Time-Traffic-Sign-Detection-main**\
├───Codes\
│ ├───models\
│ │ ├───hub\
│ │ └───__pycache__\
│ └───utils\
│ ├───google_app_engine\
│ └───__pycache__\
├───Model\
│ └───weights\
├───Results\
├───Sample Dataset\
└───Test

## Results
![Result](https://github.com/Kartik-Aggarwal/Real-Time-Traffic-Sign-Detection/blob/main/readme_images/2.PNG)
<br>
<br>
<br>
![Plots](https://github.com/Kartik-Aggarwal/Real-Time-Traffic-Sign-Detection/blob/main/readme_images/1.PNG)


## References
1. Github link to the Ultralytics repository - https://github.com/ultralytics/yolov5
2. Kaggle link for some images of the dataset - https://www.kaggle.com/andrewmvd/road-sign-detection
3. Original paper of YOLO released in May, 2016 - https://arxiv.org/pdf/1506.02640.pdf
4. Github link to the LabelImg repository - https://github.com/tzutalin/labelIm
