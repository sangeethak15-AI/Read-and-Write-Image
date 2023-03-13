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
### Developed By:Sangeetha.K
### Register Number: 212221230085
i) #To Read,display the image
```
import cv2
clr_img=cv2.imread('cat1.jpg',1)
cv2.imshow('catty',clr_img)
cv2.waitKey(0) 

```
ii) #To write the image
```
cv2.imwrite('created.jpg',clr_img)

```
iii) #Find the shape of the Image
```
print(clr_img.shape)

```
iv) #To access rows and columns

```
import random
for i in range (100):
    for j in range(clr_img.shape[1]):
        clr_img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]  
cv2.imshow('Part image',clr_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
v) #To cut and paste portion of image
```



```

## Output:

### i) Read and display the image

<br>
<br>

### ii)Write the image

<br>
<br>

### iii)Shape of the Image

<br>
<br>

### iv)Access rows and columns
<br>
<br>

### v)Cut and paste portion of image
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


