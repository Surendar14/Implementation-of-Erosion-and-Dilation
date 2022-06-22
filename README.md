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
![Screenshot (113)](https://user-images.githubusercontent.com/75235759/174993003-4f10e144-71f5-4316-865c-e8fb79ce6f19.png)

### Display the Eroded Image
![Screenshot (115)](https://user-images.githubusercontent.com/75235759/174993495-15009ed4-59c1-4c5d-a2a5-a6b6e7e9ad3c.png)

### Display the Dilated Image
![Screenshot (116)](https://user-images.githubusercontent.com/75235759/174993663-e5c461d2-c54b-44cf-895c-b2ef7297ec15.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
