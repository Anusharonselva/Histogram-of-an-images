# Histogram-of-an-images
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()

### Step2:
Print the image using imshow().



### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### Step5:
The Histogram of gray scale image and color image is shown.


## Program:
# Developed By: S.ANUSHARON
# Register Number: 212222240010
```
import cv2
import matplotlib.pyplot as plt
```
```
import cv2
import matplotlib.pyplot as plt
gray_image = cv2.imread("cha.jpeg")
color_image = cv2.imread("ch.jpeg",-1)
cv2.imshow("Gray Image",gray_image)
cv2.imshow("Colour Image",color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
```
import numpy as np
import cv2
Gray_image = cv2.imread("cha.jpeg")
Color_image = cv2.imread("ch.jpeg")
import matplotlib.pyplot as plt
gray_hist = cv2.calcHist([Gray_image],[0],None,[256],[0,256])
color_hist = cv2.calcHist([Color_image],[0],None,[256],[0,256])
plt.figure()
plt.imshow(Gray_image)
plt.show()
plt.title("Histogram")
plt.xlabel("Grayscale Value")
plt.ylabel("Pixel Count")
plt.stem(gray_hist)
plt.show()
plt.imshow(Color_image)
plt.show()
plt.title("Histogram of Color Image - Green Channel")
plt.xlabel("Intensity Value")
plt.ylabel("Pixel Count")
plt.stem(color_hist)
plt.show()
cv2.waitKey(0)
cv2.destroyAllWindows()
```
```

import cv2
gray_image = cv2.imread("cha.jpeg",0)
cv2.imshow('Grey Scale Image',gray_image)
equ = cv2.equalizeHist(gray_image)
cv2.imshow("Equalized Image",equ)
cv2.waitKey(0)
cv2.destroyAllWindows()
```




## Output:
### Input Grayscale Image and Color Image

![Screenshot 2024-03-20 100642](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/bf3ba3e7-ee9a-4391-9396-70f62b117d9b)
![Screenshot 2024-03-20 100712](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/269279ed-65e9-483b-8199-2adf01abb549)

### Histogram of Grayscale Image and any channel of Color Image
![Screenshot 2024-03-20 100806](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/ce9bd63b-2139-45a2-bf08-4bbd6e5ffdc7)
![Screenshot 2024-03-20 100837](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/9c51654f-3ae1-4266-a48d-7c0b6fbc0d41)
![Screenshot 2024-03-20 100912](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/85305fc3-8574-4beb-ba81-92e4f5239e2c)
![Screenshot 2024-03-20 100946](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/884193b4-47fa-45fe-9ffc-34c1acd1a288)



### Histogram Equalization of Grayscale Image.

![Screenshot 2024-03-20 101014](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/51d9c3c8-301d-4c38-95ca-9e158cf35b42)

![Screenshot 2024-03-20 101052](https://github.com/Anusharonselva/Histogram-of-an-images/assets/119405600/a2c611b4-2b1e-48bd-a2c5-a3804c7a94ff)


## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.

Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
