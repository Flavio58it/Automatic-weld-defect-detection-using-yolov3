# Automatic-weld-defect-detection-using-yolov3:
This app is made for detecting manufacturing weld defect from x-ray both DICOM and JPG images using yolov3 model which is finetuned over 1300 manufacturing weld defects images. 

The GUI is written in python tkinter, it is made for reading and editing DICOM and JPG images, and mainly for detecting, localizing and measuring the dimension of weld defects using deep trained YOLOV3 model.
you can download weights in this link "https://drive.google.com/file/d/1ugtEFYPN4g-LKC8t703zZSAgbZ_UwwTU/view?usp=sharing"
make sure to put both the cfg and the weights files in the same directory with the python script in order to run it.
This video shows it can be used:"https://youtu.be/4tatlyz4yFg"
# Requirements:

- python 3.7.7
- pip 20.0.2
- Pillow 7.1.1
- pydicom 2.0.0
- opencv-python 4.2.0.34
- numpy 1.19.1
- PyInstaller 3.6 (optional)

if you haven't python installed on your computer you can use the executable file directly by downloading the executable with the wieghts and the cfg file from this link "https://drive.google.com/file/d/10rYKCr1pXuuZh8AKF6P7QqYh0NCgjORl/view?usp=sharing,%20https://drive.google.com/file/d/1HJwvH21obKdhFnepyHz7TrKsspXXRDjC/view?usp=sharing" 
# Detecting defect in dicom image:
![Sans titre](https://user-images.githubusercontent.com/47951668/88341229-22db9c80-cd35-11ea-9a01-0896f93b60d8.png)
