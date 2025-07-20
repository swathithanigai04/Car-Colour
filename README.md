# **Car Colour Detection System with Traffic Analysis**

## **Overview**

This project detects the **color of cars** at traffic signals and counts the number of cars and people present. It also uses a **bounding box system** for visualization:

* **Red box** → Blue-colored cars.
* **Blue box** → Cars of other colors.

If people are detected at the traffic signal, the system displays the **number of individuals present**.
The application includes a **Graphical User Interface (GUI)** that allows users to upload an image or video and view the detection results in real time.


## **Features**

* Detect multiple cars and classify their colors.

* Highlight blue cars with **red bounding boxes** and others with **blue boxes**.

* Count the total number of cars at a traffic signal.

* Detect and display the number of people in the image/video.

* User-friendly **Tkinter GUI** with:

  * **Image Input**
  * **Video Input**
  * **Real-time Preview**

* Models trained using **Transfer Learning (MobileNetV2)** for color classification.

## **requirements.txt**

```
tensorflow>=2.12.0
keras>=2.12.0
opencv-python
numpy
pandas
matplotlib
scikit-learn
pillow
tkintertable
```

## **Model Details**

* **Car Color Classification Model**:

  * Built using **MobileNetV2** with fine-tuning.
  * Trained on a dataset of different car colors with augmentation.
* Performance:

  * Color Classification Accuracy: **78%**
  * Evaluated using **Confusion Matrix**, **Precision**, and **Recall**.
   
##  **Model File**

The trained model file car_color_classifier.h5 is included in the repository.
Since the file size exceeds GitHub limits, download it from **\[Google Drive link]** (https://drive.google.com/file/d/1GnLz31m5_tL1uXk2zcK5vyOj66iKv3dp/view?usp=sharing).

## **Outputs**

* Real-time bounding boxes on cars:

  * **Red** → Blue cars.
  * **Blue** → Other color cars.
* Displays:

  * **Car count**
  * **People count**.

## **Future Improvements**

* Add **real-time camera stream integration**.
* Support for **multiple car models and detection in crowded frames**.
* Deploy as a **mobile app or web application** for traffic monitoring systems.
