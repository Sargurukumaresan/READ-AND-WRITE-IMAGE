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
### Developed By:SARGURU K
### Register Number: 212222230134
i) #To Read,display the image
```
import cv2
image=cv2.imread("image1.png",1)
cv2.imshow('212222230134_SARGURU',image)
cv2.waitKey(0) 
```
ii) #To write the image
```
import cv2
image=cv2.imread("image1.png",1)
w=cv2.imwrite('i.png',image)
cv2.imshow('212222230134_SARGURU',image)
cv2.waitKey(0) 
```
iii) #Find the shape of the Image
```python3
import cv2
import random
image=cv2.imread("image1.png",1)
print(image.shape)
```
iv) #To access rows and columns

```python3
import cv2
import random
image=cv2.imread("image1.png",1)

for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222230134_SARGURU',image)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```python3
import cv2

image=cv2.imread("image1.png",1)
image.shape
tag=image[350:550,200:350]
image[70:270,200:350]=tag
cv2.imshow('212222230134_SARGURU',image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image
![S1](https://github.com/Sargurukumaresan/READ-AND-WRITE-IMAGE/assets/119559840/be99fd77-f021-4ef0-b63c-fd2faf3f1f88)


### ii)Write the image
![S2](https://github.com/Sargurukumaresan/READ-AND-WRITE-IMAGE/assets/119559840/fd051d83-ade6-41fe-994d-e6450ac4a4c9)


### iii)Find the shape of the Image
![S3](https://github.com/Sargurukumaresan/READ-AND-WRITE-IMAGE/assets/119559840/f8f4f454-b74a-4160-92ad-1460f0c2cce7)



### iv)Access rows and columns
![S4](https://github.com/Sargurukumaresan/READ-AND-WRITE-IMAGE/assets/119559840/8e816c86-c13b-436b-b151-83fe536662cd)



### v)Cut and paste portion of image
![S5](https://github.com/Sargurukumaresan/READ-AND-WRITE-IMAGE/assets/119559840/c818a0ce-3d5a-4d70-a1c9-1ec6b4c4c889)



## Result:
Thus the images are read, displayed, and written successfully using the python program.
