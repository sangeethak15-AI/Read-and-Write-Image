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
tag = clr_img[300:400,300:400]
clr_img[50:150,50:150] = tag
cv2.imshow('part of image',clr_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image

![Screenshot 2023-03-13 203918](https://user-images.githubusercontent.com/93992063/225051542-c5371946-3909-46d8-9187-412eeb6c583b.png)


### ii)Write the image

![Screenshot 2023-03-13 204029](https://user-images.githubusercontent.com/93992063/225051590-1a9448ec-36f0-4b47-adfc-7b26b34cf9f6.png)


### iii)Shape of the Image


![Screenshot 2023-03-13 204109](https://user-images.githubusercontent.com/93992063/225051617-5c539302-1a02-46d4-aedd-085d4b2d0cf9.png)

### iv)Access rows and columns

![Screenshot 2023-03-13 204306](https://user-images.githubusercontent.com/93992063/225051679-2f211072-b6d4-46d9-be79-0aff848256cd.png)


### v)Cut and paste portion of image
![Screenshot 2023-03-14 135456](https://user-images.githubusercontent.com/93992063/225051815-906279b7-94f0-4380-b893-ee9cd70582bf.png)



## Result:

Thus the images are read, displayed, and written successfully using the python program.


