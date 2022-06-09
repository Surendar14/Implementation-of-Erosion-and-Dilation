# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
### Step2:
Create the Text using cv2.putText.
### Step3:
Create the structuring element.
### Step4:
Erode and Dilate the image.
### Step5:
End Program.
## Program:
``` Python
# Developed By   : SURENDAR S
# Register Number: 212220230051
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1 = np.zeros((100,270), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'aakaash',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')

# Create the structuring element
cv2.erode(img1, kernel)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
image_erode1 = cv2.erode(img1,kernel)
plt.imshow(image_erode1, 'gray')

# Dilate the image
image_dilate1 = cv2.dilate(img1, kernel)
plt.imshow(image_dilate1, 'gray')
```
## Output:
### Display the input Image
![01](https://user-images.githubusercontent.com/75235747/169687674-013d5012-ede3-4006-968e-7dcafa1ad94a.JPG)
### Display the Eroded Image
![02](https://user-images.githubusercontent.com/75235747/169687684-098631c1-fd5a-4936-a30a-ba72efede5a6.JPG)
### Display the Dilated Image
![03](https://user-images.githubusercontent.com/75235747/169687700-fd3fa97a-e82a-418a-b002-8692cd01394e.JPG)
## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
