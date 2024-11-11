#  Ex 9 - Implementation of Erosion and Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1:
Import the required libraries.
### Step 2: 
Create a text image using cv2.putText().
### Step 3: 
Define a structuring element for the erosion and dilation operations.
### Step 4: 
Apply erosion to the image using cv2.erode().
### Step 5: 
Apply dilation to the image using cv2.dilate().
### Step 6: 
Display the original, eroded, and dilated images.
 
## Program:
### Developed by : SWATHI D
### Reg.no : 212222230154
``` Python
# Import the necessary packages
import cv2
import numpy as np
image = np.zeros((300, 600), dtype="uint8")

# Create the Text using cv2.putText
cv2.putText(image, 'Image Processing', (30, 150), cv2.FONT_HERSHEY_SIMPLEX, 2, (255, 255, 255), 5)

# Create the structuring element
kernel = np.ones((5,5), np.uint8)

# Erode the image
eroded_image = cv2.erode(image, kernel, iterations=1)

# Dilate the image
dilated_image = cv2.dilate(image, kernel, iterations=1)

cv2.imshow('Input Image', image)
cv2.imshow('Eroded Image', eroded_image)
cv2.imshow('Dilated Image', dilated_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## Output:

### Display the input Image
![Screenshot 2024-10-21 161614](https://github.com/user-attachments/assets/dae657f6-7ac6-4781-8f5b-5f8625e9c0cc)


### Display the Eroded Image
![Screenshot 2024-10-21 161605](https://github.com/user-attachments/assets/4f1ebf18-10c0-4172-bb7c-36bfd35b3a62)


### Display the Dilated Image
![Screenshot 2024-10-21 161556](https://github.com/user-attachments/assets/45c080ee-dc8a-48d0-822f-9b9f8be6f249)



## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
