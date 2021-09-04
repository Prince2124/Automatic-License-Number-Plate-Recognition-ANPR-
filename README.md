# Automatic-License-Number-Plate-Recognition-ANPR-
Automatic Number Plate Recognition (ANPR) is commonly used in many countries for many applications like Ticketless parking fee management, car theft prevention etc. ANPR systems consists of three stages:  Car Plate Detection with OpenCV and Haar Cascade,  Plate Number Recognition and Extraction with TesseractOCR.


![image](https://user-images.githubusercontent.com/59818604/132103398-52d91c75-cb0b-4b91-9239-c9e33a8bc47b.png)

# Model (Haar Cascades)
OpenCV actually comes with pre-trained XML files of various Haar Cascades, where each XML file contains the feature set. We will be using the Haar Cascade XML file containing the features for Russian car plates, and here’s how you can download the Haar Cascade XML file from: https://raw.githubusercontent.com/opencv/opencv/master/data/haarcascades/haarcascade_russian_plate_number.xml

# TesseractOCR
TesseractOCR is an open source optical character recognition (OCR) engine. It is recognized as one of the most popular and most accurate open-source OCR engines. 

# Execution steps
A. We convert input image into to gray-scale to reduce the noises.
B. And then use haar cascade classifire model to detectect lisence plate and get the cordinates of ROI(Plate).
C. Apply image preprocessing over plate Smoothing (blurring or de-noising) then pass to pytesseracrt to grt the text.
D. After de-noising the plate pass it to pytesseracrt to get the text.

# Results
A. Cropped plate:

![cropped plate1](https://user-images.githubusercontent.com/59818604/132103726-b09fe3ae-2035-4745-8e09-b4a42c216944.png)

![cropped plate2](https://user-images.githubusercontent.com/59818604/132103714-b269beaf-5771-409c-b486-a3780adef221.png)

B. Detected number plate

![result](https://user-images.githubusercontent.com/59818604/132103767-7facfc58-7c0f-4a79-9fb0-ec88ae3fda99.png)

![result1 (2)](https://user-images.githubusercontent.com/59818604/132103785-1974b5ad-c9c9-4ee3-b295-d8c47ef778a6.jpg)

![result1 (1)](https://user-images.githubusercontent.com/59818604/132103875-686385c1-f4bd-4392-afad-5d598130c558.jpg)


# References
https://towardsdatascience.com/russian-car-plate-detection-with-opencv-and-tesseractocr-dce3d3f9ff5c
