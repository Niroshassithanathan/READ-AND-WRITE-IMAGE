# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:NIROSHA S
### Register Number:212222230097 
i) #To Read,display the image
```
import cv2 as cv
capture=cv.imread("cat.jpg")
cv.imshow('212222230097_NIROSHA S',capture)
cv.waitKey(0)

```
ii) #To write the image
```
import cv2 as cv
capture=cv.imread("cat.jpg")
cv.imwrite("photo.jpg",capture)
cv.imshow("212222230097_NIROSHA S",capture)
cv.waitKey(0)
```
iii) #Find the shape of the Image
```
import random
import cv2 as cv
capture=cv.imread("cat.jpg")
print(capture.shape)
```
iv) #To access rows and columns

```
import random
import cv2 as cv
capture=cv.imread("cat.jpg")
for i in range(70,90):
    for j in range(110,170):
        capture[i][j]=[0,0,0]
cv.imshow("212222230097_NIROSHA S",capture)
cv.waitKey(0)
```
v) #To cut and paste portion of image
```
import random
import cv2 as cv
capture=cv.imread("cat.jpg")
tag=capture[100:120,110:120]
capture[0:20,10:20]=tag
cv.imshow("212222230097_NIROSHA S",capture)
cv.waitKey(0)
```

## Output:

### i) Read and display the image

![cat1](https://github.com/Niroshassithanathan/READ-AND-WRITE-IMAGE/assets/121418437/a38ea308-b26d-4338-aee4-098097095328)

### ii)Write the image

![cat2](https://github.com/Niroshassithanathan/READ-AND-WRITE-IMAGE/assets/121418437/fcb73758-d0b8-4f97-af8d-236143f05af0)

### iii)Shape of the Image

![cat3](https://github.com/Niroshassithanathan/READ-AND-WRITE-IMAGE/assets/121418437/3b0f0ab1-41d5-4500-bd19-2186a4d709b4)

### iv)Access rows and columns

![cat4](https://github.com/Niroshassithanathan/READ-AND-WRITE-IMAGE/assets/121418437/877d94bc-0265-4bac-9b08-6fe6300816d8)

### v)Cut and paste portion of image

![cat5](https://github.com/Niroshassithanathan/READ-AND-WRITE-IMAGE/assets/121418437/be639837-4f3e-415b-833e-f17ab452702e)

## Result:
Thus the images are read, displayed, and written successfully using the python program.
