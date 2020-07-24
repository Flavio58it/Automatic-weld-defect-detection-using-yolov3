# Automatic-weld-defect-detection-using-yolov3:
This app is made for detecting manufacturing weld defect from x-ray images both DICOM and JPG images using yolov3 custom detection model which is trained over 1300 manufacturing weld defects. 

The GUI is written in python tkinter, it is made for reading and editing DICOM and JPG format, and mainly for detecting, localizing and measuring the length of weld defects using deep learning YOLOV3 trained model.
you can download weights from this link "https://drive.google.com/file/d/1ugtEFYPN4g-LKC8t703zZSAgbZ_UwwTU/view?usp=sharing"
make sure to put both the cfg and weights  files in the same directory with the executable in order to run this app

# Requirements:

- python 3.7.7
- Pillow 7.1.1
- pydicom 2.0.0
- pip 20.0.2
- opencv-python 4.2.0.34
- numpy 1.19.1
- PyInstaller 3.6 (optional)

if you haven't python installed you can use the exe file directly by downloading the executable file from this link 
#enjoy!!
# Detecting defect in dicom image:
![Sans titre](https://user-images.githubusercontent.com/47951668/88341229-22db9c80-cd35-11ea-9a01-0896f93b60d8.png)
