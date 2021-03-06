# Pothole Detection System (image or video)
##               by The_Newcomers
### Read ppt for overview

This model is a deep learning model using YOLO v2.

It has been trained for ~125 images and the accuracy would get better with larger database.

For Pre Trained wts : - https://drive.google.com/file/d/1zzlyFlb8wzEHAURy_pstzPvuDlPaXU1S/view?usp=sharing

Run `pip install -r requirements.txt` in the potholes_detection detection folder. Then for tensorflow: -

For local running use: - tensorflow-gpu==1.15 , CUDA V 10.0 , cuDNN V 7.6.5  ( https://www.tensorflow.org/install/gpu#software_requirements )
(tip use a new virtual env using pycharm or something and select basic interpreter as conda python 3.6 and then install everything.)

For Google Colabs (easier to run) just use : - tensorflow-gpu==1.14

#### To run: - 
```
python predict.py -c config.json -w /path/of/trained_wts.h5 -i /path/of/image(jpg or png)/or/video(mp4)
```

### Example
![Road with potholes](potholes_detection/images/pothole2.png?raw=true "Road with Potholes")
### Detected potholes: -
![Road with potholes detected](potholes_detection/images/pothole2_detected.png?raw=true "Road with Potholes")

#### Note: - The front end(django) is yet to be connected to the backend.
