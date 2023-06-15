# EX-10--Implementation-of-Erosion-and-Dilation
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

```
# Developed By   : SURENDAR S
# Register Number: 212220230051
```

``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
image = np.zeros((100,290), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image,'Surendar',(3,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(image, 'plasma')

# Create the structuring element
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
cv2.erode(image, kernel)

# Erode the image
image_erode1 = cv2.erode(image,kernel)
plt.imshow(image_erode1,'plasma')

# Dilate the image
image_dilate1 = cv2.dilate(image, kernel)
plt.imshow(image_dilate1,'plasma')
```
## Output:
### Display the input Image

![text](https://user-images.githubusercontent.com/75235759/235293202-afbae223-99af-4ff3-a1c3-ae502beab728.png)

### Display the Eroded Image

![erode1](https://user-images.githubusercontent.com/75235759/235293211-bad1863d-d307-4bf2-933c-c2c66635b773.png)

### Display the Dilated Image

![dilate1](https://user-images.githubusercontent.com/75235759/235293216-687729f8-9a40-4c1d-8ad2-e4acbb1b86b8.png)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
