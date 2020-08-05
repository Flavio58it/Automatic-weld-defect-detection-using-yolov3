# Automatic-weld-defect-detection-using-yolov3:
In non-destructive testing (NDT) the use of  X-ray weld defect images for defects detection is a very significant method. Traditionally, this work had to be done by skilled technicians who are time-consumed and easily influenced by the environment. Many efforts have been made on automatic classification. However their work either need manual features specified by technicians or get a low accuracy. In this work I have customize the famous YOLOv3 pre-trained weights (https://pjreddie.com/darknet/yolo/) to detect weld defects, instead of the 20 classes which are the original model has been trained on, I used only one class named “defaut” containing many type of defects  (Cracks, Blow holes, Solid inclusion). The original YOLOv3 has mAP measured at 0.5 IOU = 60.6 % on COCO dataset "https://cocodataset.org", while on my small local dataset (1300 samples) I have gotten mAP =83.35 % in the same IOU value. I have deployed that model on a windows desktop application which is made for detecting manufacturing weld defect from x-ray both DICOM and JPG images, whith the ability of browsing and saving the result as JPG or PNG image
The GUI is written in python tkinter, it can read and edit  DICOM and JPG images, and mainly  detect, localize and measure length of the weld defect detected.
You can download weights separately  in this link https://drive.google.com/uc?id=1ugtEFYPN4g-LKC8t703zZSAgbZ_UwwTU&export=download , just make sure to put both the cfg and the pre-trained weights in the same directory with the python script in order to run it.

# Video
This video shows the source code and short tutorial about the app :https://www.youtube.com/watch?v=qZkWvCNbpZM
# Requirements:
Despite the use of deep pre-trained model “YOLOv3”, the trained model deployment doesn’t require to install any of deep learning libraries like Tensorflow, Keras or even darknet framework which is necessary for training, this App is simply use opencv for deployment: 
- python 3.7.7
- pip 20.0.2
- Pillow 7.1.1
- pydicom 2.0.0
- opencv-python 4.2.0.34
- numpy 1.19.1
- PyInstaller 3.6 (optional)
# The .exe file:
if you haven't python installed on your computer you can use the executable file directly by downloading it with the weights and cfg file in here https://drive.google.com/file/d/10rYKCr1pXuuZh8AKF6P7QqYh0NCgjORl/view
# Detecting defect in dicom image:
![Sans titre](https://user-images.githubusercontent.com/47951668/88341229-22db9c80-cd35-11ea-9a01-0896f93b60d8.png)
 # Perspective
 - I will gather more training data to improve the mAP and the accuracy 
 - I will augment the number of classes to be 7 different classes equally to weld defects types which will make the app more useful  
 - I will use PYQt5 instead of tkinter in order to improve the GUI design
 # Contact 
 b.yassine.89@gmail.com
