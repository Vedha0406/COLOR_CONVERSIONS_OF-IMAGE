# COLOR_CONVERSIONS_OF-IMAGE
## AIM
Write a Python program using OpenCV that performs the following tasks:

i) Read and Display an Image.

ii) 	Draw Shapes and Add Text.

iii) Image Color Conversion.

iv) Access and Manipulate Image Pixels.

v) Image Resizing

vi) Image Cropping

vii) Image Flipping

viii)	Write and Save the Modified Image


## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Load an image from your local directory and display it.
### Step2:
o	Draw a line from the top-left to the bottom-right of the image.
o	Draw a circle at the center of the image.
o	Draw a rectangle around a specific region of interest in the image.
o	Add the text "OpenCV Drawing" at the top-left corner of the image.

### Step3:
o	Convert the image from RGB to HSV and display it.
o	Convert the image from RGB to GRAY and display it.
o	Convert the image from RGB to YCrCb and display it.
o	Convert the HSV image back to RGB and display it.

### Step4:
o	Access and print the value of the pixel at coordinates (100, 100).
o	Modify the color of the pixel at (200, 200) to white.

### Step5:
o	Resize the original image to half its size and display it.
### Step6:
o	Crop a region of interest (ROI) from the image (e.g., a 100x100 pixel area starting at (50, 50)) and display it.
### Step7:
o	Flip the original image horizontally and display it.
o	Flip the original image vertically and display it.

### Step8:
o	Save the final modified image to your local directory.


##### Program:COLOR CONVERSION OF IMAGE
### Developed By:VEDHAHSREE.G
### Register Number212223240171


## Output:

### i)Read and Display an Image

import cv2

image=cv2.imread('example.png',1)

image = cv2.resize(image, (500, 300))4

cv2.imshow('example2.png',image)

cv2.waitKey(0)

cv2.destroyAllWindows()

![image](https://github.com/user-attachments/assets/dc52b3e6-c470-4298-98e6-23a4b047a115)




### ii)Draw Shapes and Add Text

cv2.imwrite('example.png',image)
![write image](https://github.com/user-attachments/assets/e27a4937-c7f9-41df-8db2-922234bedd8d)


### iii)Image Color Conversion


image.shape

![image](https://github.com/user-attachments/assets/cfe54f95-22b9-4595-80d3-0bb073ecbfa5)

### iv)Access and Manipulate Image Pixels
```
import random
image=cv2.resize(image,(400,400))
for i in range (150,200):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),
                    random.randint(0,255),
                    random.randint(0,255)]
cv2.imshow('murugar',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
![image](https://github.com/user-attachments/assets/0620f27f-77ef-46cd-b161-9a6c6acef401)
```

### v)Image Resizing
```
image=cv2.imread('example.png',1)
image=cv2.resize(image,(400,400))
tag =image[130:200,110:190]
image[110:180,120:200] = tag
cv2.imshow('murugar',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
![image](https://github.com/user-attachments/assets/07f134ab-9ac5-4e2a-bbb3-cc2c2bc5ad82)
```

### vi)Image Cropping


### vii)Image Flipping
<br>
<br>

### viii)Write and Save the Modified Image
<br>
<br>






## Result:
Thus the images are read, displayed, and written ,and color conversion was performed  successfully using the python program.







