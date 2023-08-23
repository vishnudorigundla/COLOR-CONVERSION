# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
import opencv.

### Step2:
Read the original Image.

### Step3:
Store the required conversion of the image in a variable.

### Step4:
Show the image stored in the given variable.

### Step5:
Destroy all the windows and end the program.

## Program:
```
Developed By : D.vishnu vardhan reddy
Register Number : 212221230023
```
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('bike.jpeg')
cv2.imshow('Original Image',houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

# ii)Convert HSV to RGB and BGR

```
import cv2
house_HSV_image= cv2.imread('bike.jpeg')
cv2.imshow('Original HSV image',house_HSV_image)
RGB_image = cv2.cvtColor(house_HSV_image, cv2.COLOR_HSV2RGB)
cv2.imshow('HSV to RGB',RGB_image )
BGR_image = cv2.cvtColor(house_HSV_image, cv2.COLOR_HSV2BGR)
cv2.imshow('HSV to BGR',BGR_image)
cv2.waitKey(0)
cv2.destroyAllwindows()
​
```



# iii)Convert RGB and BGR to YCrCb

```
import cv2
houseImage = cv2.imread('bike.jpeg')
cv2.imshow('Original HSV Image',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```


# iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('bike.jpeg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



# v) Split and merge HSV Image
```
import cv2
image = cv2.imread('bike.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
## Output:
### i) BGR and RGB to HSV and GRAY
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/5ec2c297-5ce5-4fc1-a7b7-0e7ea1247d2f)

![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/6abd3b5d-c842-4b69-9561-3caf1d607fa1)

![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/46618359-7b45-4e2e-a2ec-ec79f9063798)

![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/4019cdc0-a6f6-491f-be61-76b13a9117e5)

![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/4021e3da-6995-4c6a-96a8-24066b5cc3ad)

### ii) HSV to RGB and BGR

![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/9f35e4b1-52e0-4539-b5eb-563e5c7bb0b7)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/04f2f35d-f135-41f3-83c9-2ec33ae38dd7)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/1ad61816-7ba2-4c2c-aebb-b7dceb551539)



### iii) RGB and BGR to YCrCb
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/2d57d319-6ad5-4eeb-8cb5-7e1edffa98ee)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/707cf7dd-9608-4496-a8ee-25555480bc8b)

![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/91e0ce62-7e66-4119-96d3-5d772de5696a)
### iv) Split and merge RGB Image
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/e082ebfe-2608-46f6-bdb2-b672ceff44dd)

![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/a84adcd3-09ec-41b4-a416-a76a936f0d39)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/b95d3f56-52b8-43f2-90d4-9eda30b561d6)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/a26bef49-11a1-4d47-ade9-9eaf5502d967)

### v) Split and merge HSV Image
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/dcdb726d-d403-44de-9026-f26bfe0e281b)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/1e65b919-bfa7-4316-876f-cd605b93f0c3)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/abe0c96f-881b-4ab8-b697-c1531a84ad23)
![image](https://github.com/vishnudorigundla/COLOR-CONVERSION/assets/94175324/75616310-7f4f-4ac8-83b5-4c1dbce8d3ab)


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
