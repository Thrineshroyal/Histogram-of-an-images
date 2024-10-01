# Histogram-of-an-images
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()

### Step2:
Print the image using imshow().

### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### Step5:
The Histogram of gray scale image and color image is shown.


## Program:
### Developed By: Thrinesh Royal
### Register Number: 212223230226
### Input Grayscale Image and Color Image
## Gray Image:
```
import cv2
import matplotlib.pyplot as plt
image = cv2.imread('devara.jpeg')
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
plt.imshow(gray_image, cmap='gray')
plt.title('Original Grayscale Image')
plt.axis('on')
```
![Screenshot 2024-10-01 112958](https://github.com/user-attachments/assets/0304c371-5a5e-4550-bbd1-85a1c12226db)


### Histogram of Grayscale Image and any channel of Color Image
## Histrogram:
```p
plt.plot(hist_original, color='black')
plt.title('Original Histogram')
plt.xlim([0,256])
```
## OUTPUT:

![Screenshot 2024-10-01 113127](https://github.com/user-attachments/assets/9bfb60b1-a095-4e99-a36d-a2afea0e40b3)

### Histogram Equalization of Grayscale Image.

## Equalized Image:
```
equalized_image = cv2.equalizeHist(gray_image)
plt.imshow(equalized_image, cmap='gray')
plt.title('Equalized Image')
plt.axis('on')
```
## OUTPUT:
![Screenshot 2024-10-01 113216](https://github.com/user-attachments/assets/11d2cb84-aec0-4c1e-bb49-9cb50a393ced)


## Histrogram:
```
plt.plot(hist_equalized, color='black')
plt.title('Equalized Histogram')
plt.xlim([0, 256])
```
## OUTPUT:
![Screenshot 2024-10-01 113310](https://github.com/user-attachments/assets/a9477b36-d753-447b-a673-7d8af829c802)

## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
