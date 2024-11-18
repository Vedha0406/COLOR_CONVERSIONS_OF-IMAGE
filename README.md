# EX-1 COLOR_CONVERSIONS_OF-IMAGE
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
```
import cv2
image=cv2.imread('c.jpg',1)
cv2.imshow('Image Window', image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/1a1f2cce-f13c-438d-aeee-e7a75eea56fe)

### ii)Draw Shapes and Add Text
```
import cv2
img = cv2.imread("example.png")
res = cv2.line(img, (0, 0), (599, 799), (200, 100, 205), 10)
cv2.imshow('Image Window', res)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/153a0448-6b18-498c-a61d-b414e6972d56)
)

ii)Draw a circle at the center of the image.
```
import cv2

# Load the image
img = cv2.imread("example.png")

# Get the dimensions of the image
height, width, _ = img.shape

# Calculate the center of the image
center_coordinates = (width // 2, height // 2)

# Draw a circle at the center of the image
res = cv2.circle(img, center_coordinates, 150, (255, 0, 0), 10)

# Display the image with the circle
cv2.imshow('Image Window', res)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/fe83f22f-efc8-417d-b045-370c98da8d33)

### iii)Image Color Conversion

### RGB to HSV AND  RGB to GRAY
```
img = cv2.imread('example.png',1)
img = cv2.resize(img,(300,200))
cv2.imshow('Original Image',img)
hsv1 = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsv1)
hsv2 = cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsv2)
gray1 = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',gray1)
gray2 = cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',gray2)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/b00435d4-2f30-4762-abd5-fd2f3a0a43de)
![image](https://github.com/user-attachments/assets/1ee63c85-fe25-434f-99cb-57c753faaf34)
![image](https://github.com/user-attachments/assets/b18b46af-905f-414f-aaa8-dd3a186393f1)
![image](https://github.com/user-attachments/assets/10988290-1d45-4223-a86a-3f058958b650)

### RGB to YCrCb 
```
img = cv2.imread('example.png')
img = cv2.resize(img,(300,200))
cv2.imshow('Original RGB Image',img)
YCrCb1 = cv2.cvtColor(img, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB-2-YCrCb',YCrCb1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/2cf5a45a-4d29-4474-8a43-15565a0b83cc)
![image](https://github.com/user-attachments/assets/10ea745d-bda9-4213-b112-183f1e891fe0)

### HSV image back to RGB
```
hsv_image = cv2.imread("example.png")
rgb_image = cv2.cvtColor(hsv_image, cv2.COLOR_HSV2BGR)
cv2.imshow('RGB Image', rgb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/788a3f9b-b4ea-45c0-96e2-8f4364d07889)


### iv)Access and Manipulate Image Pixels
```
![image](https://github.com/user-attachments/assets/1989a6a7-cd73-4736-8e35-2a6ef4dd79d3)

![image](https://github.com/user-attachments/assets/caa8c681-d998-434a-9cd3-0eab383f41a4)
```

 ### Image Resizing
 ```
import cv2
image = cv2.imread("example.png")
height, width = image.shape[:2]
half_size_image = cv2.resize(image, (width // 2, height // 2))
cv2.imshow('Resized Image (Half Size)', half_size_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/0d865fa1-6042-4612-95b0-fdeb08300773)

### vi)Image Cropping
```
image=cv2.imread('example.png',1)
image=cv2.resize(image,(400,400))
tag =image[130:200,110:190]
image[110:180,120:200] = tag
cv2.imshow('murugar',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/07f134ab-9ac5-4e2a-bbb3-cc2c2bc5ad82)

### vii)Image Flipping
### HORIZONTAL FLIPPING
```
import cv2
image = cv2.imread("example.png")
flipped_image = cv2.flip(image, 1)
cv2.imshow('Flipped Image', flipped_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### VERTICAL FLIPPING
```
import cv2
image = cv2.imread("example.png")
flipped_image = cv2.flip(image, 0)
cv2.imshow('Flipped Image', flipped_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
![image](https://github.com/user-attachments/assets/bb7a8d49-2bd5-42c3-ba62-ff73322f6933)
![image](https://github.com/user-attachments/assets/a2cc8219-034f-470b-8891-0db9104cddb7)

### viii)Write and Save the Modified Image

![image](https://github.com/user-attachments/assets/58dfc7b8-be8a-4a61-9335-ef3acff8df6c)

## Result:
Thus the images are read, displayed, and written ,and color conversion was performed  successfully using the python program.







