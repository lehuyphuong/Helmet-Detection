# Streamlit-project: Helmet-Detection
## **Overview**
This project focuses on building helmet safety monitoring using model YOLOv10
and streamlit as GUI.
The rest content of this article guide how to set up, train model and run.
Depending on what you prefer, you can choose either part 1 or part 2.

### **Part 1: Train model**
This part will focus on:
* Install libraries
* Load dataset
* Train model
> Note: The article has already done training model, you can move to part 2 if you want to

### *Prerequisites*
The following steps are for establishing environment:
1. Install python (3.10.14), you can download from this link:
[python.org](http://~https://www.python.org/downloads/)
2. Clone Yolov10 model:
```
    !git clone https://github.com/THU-MIG/yolov10.git
```
3. Navigate to Yolo folder:
```
    %cd yolov10
```
4. Install Python dependences:
```
    !pip install -q -r requirements.txt
    !pip install -e
```
5. Download pre-trained model:
```
    !wget https://github.com/THU-MIG/yolov10/releases/download/v1.1/yolov10n.pt
```
6. Download dataset: You can download from here: 
[safety_helmet_dataset](https://drive.google.com/file/d/1twdtZEfcw4ghSZIiPDypJurZnNXzMO7R/view)

7. Unzip dataset
8. Train model: take this file [train.py](../Helmet-detection/yolov10/train.py) and put them in folder yolov10. Then, run it.
9. Test model: take this file [test.py](../Helmet-detection/yolov10/test.py) and put them in folder yolov10. Then, run it.

### **Part 2: Demo project**
This part will focus on:
* Install dependencies
* Set up Streamlit and Load model
* Run steamlit

### *Prerequisites*
1. Install python packages:
```
    pip install streamlit
    pip install numpy
```
2. Set up streamlit, load model and run: take file [helmet_detection.py](../Helmet-detection/yolov10/helmet_detection.py).
and put them in folder yolov10.

3. Run helmet_detection.py by streamlit:
```
    streamlit run helmet_detection.py
``` 