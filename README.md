# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
<br>

### Step2:
<br>

### Step3:
<br>

### Step4:
<br>

### Step5:
<br>

## Program:
```
# Developed By:Vishranthi A
# Register Number:212221230124
```
# Read the image
```python
import cv2
img= cv2.imread('taj.jpg',1)
```
# i) Convert BGR and RGB to HSV and GRAY
## BGR to HSV
```python
cv2.imshow('Original',img)
hsvimg=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR-hsv',hsvimg)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## RGB to HSV
```python
cv2.imshow('Original',img)
hsvimg1=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB-hsv',hsvimg1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## BGR to GRAY
```python
cv2.imshow('Original',img)
gray1=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('gray-BGR',gray1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## RGB to GRAY
```python
cv2.imshow('Original',img)
gray=cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imshow('gray-RGB',gray)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# ii)Convert HSV to RGB and BGR
## HSV to RGB
```python
cv2.imshow('HSV',hsvimg)
rgb_img=cv2.cvtColor(hsvimg,cv2.COLOR_HSV2RGB)
cv2.imshow('hsv2rgb',rgb_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## HSV to BGR
```python
cv2.imshow('HSV',hsvimg)
bgr_img=cv2.cvtColor(img,cv2.COLOR_HSV2BGR)
cv2.imshow('hsv2bgr',bgr_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# iii)Convert RGB and BGR to YCrCb
## RGB to YCrCb
```python
cv2.imshow('Original',img)
YCrCb_image = cv2.cvtColor(img, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB_YCRCB',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## BGR to YCrCb
```python
cv2.imshow('Original',img)
YCrCb_image = cv2.cvtColor(img, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR_YCRCB',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# iv)Split and Merge RGB Image
```python
import cv2
img=cv2.imread('eiffel.jfif')
blue=img[:,:,0]
green=img[:,:,1]
red=img[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
merged_BGR=cv2.merge((blue,green,red))
cv2.imshow('Merged BGR Image',merged_BGR)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# v) Split and merge HSV Image
```python
hsv = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
h,s,v=cv2.split(hsv)
cv2.imshow("Hue-image",h)
cv2.imshow("Saturation-image",s)
cv2.imshow("Gray-image",v)
Merged_HSV=cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',Merged_HSV)
cv2.waitKey(0)
cv2.destoryAllWindows()
```
## Output:
### i) BGR and RGB to HSV and GRAY
## BGR to HSV
![2](https://user-images.githubusercontent.com/93427278/228274281-0d9ef1eb-e4b7-49d1-b902-572c108e62a0.png)

<br>

## RGB to HSV
![3](https://user-images.githubusercontent.com/93427278/228274413-09b7963e-4934-47fa-bd9d-2bb9ef90bf1f.png)
<br>

## BGR to GRAY
![4](https://user-images.githubusercontent.com/93427278/228274519-22d62756-0584-43a6-917c-bbc549337f74.png)

<br>

## RGB to GRAY
![5](https://user-images.githubusercontent.com/93427278/228274674-a70eb837-6ad8-4217-825f-218adc7d685d.png)
<br>

### ii) HSV to RGB and BGR
## HSV to RGB
![Screenshot (32)](https://user-images.githubusercontent.com/93427278/228271350-52a6e5c8-e6a2-4e79-872b-093ceb613513.png)

<br>

## HSV to BGR
![Screenshot (33)](https://user-images.githubusercontent.com/93427278/228271405-7cefbb7e-383b-4ef2-89cb-26a443b76fba.png)

<br>

### iii) RGB and BGR to YCrCb
## RGB to YCrCb
![Screenshot (34)](https://user-images.githubusercontent.com/93427278/228271756-d0ec800e-7354-487f-a5cd-b521695e975c.png)

<br>

## BGR to YCrCb
![Screenshot (35)](https://user-images.githubusercontent.com/93427278/228271843-6b7c5420-b2bb-486c-8692-6a8b2da5d569.png)

<br>

### iv) Split and merge RGB Image
![Screenshot (36)](https://user-images.githubusercontent.com/93427278/228271989-1b45f0dc-9a5e-46bb-9ea3-dbcabc6a8a73.png)

<br>

### v) Split and merge HSV Image
![Screenshot (37)](https://user-images.githubusercontent.com/93427278/228272235-7d3c299b-1be5-4eab-b58b-2726a198644b.png)

<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
