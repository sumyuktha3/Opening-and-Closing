# OPENING AND CLOSING

## AIM:
To implement Opening and Closing using Python and OpenCV.

## SOFTWARE REQUIRED:
1. Anaconda - Python 3.7
2. OpenCV
## ALGORITHM:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Use Opening operation.
### Step 5:
Use Closing Operation.

<br><br><br><br><br>

# PROGRAM:
## Developed by   : S.Sumyuktha Rani
## Register Number: 212220230050

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'SUM',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```
# Create the structuring element
```
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```
# Use Opening operation
```
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```
# Use Closing Operation
```
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()

```
## OUTPUT:

### Display the input Image

![sa1](https://user-images.githubusercontent.com/75235818/171091855-7f0e83ca-f33a-4f36-8e92-21eac558db23.jpg)

### Display the result of Opening

![sa2](https://user-images.githubusercontent.com/75235818/171091863-feacee50-a090-4931-9cf7-268fadffddee.jpg)

### Display the result of Closing

![sa3](https://user-images.githubusercontent.com/75235818/171091871-d6f96da5-8113-419e-be89-31cdc8881f65.jpg)

## RESULT:
Thus the Opening and Closing operation is used in the image using python and OpenCV.
