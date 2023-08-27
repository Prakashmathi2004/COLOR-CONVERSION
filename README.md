# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import cv2 library and upload the image or capture an image.

### Step2:
Read the saved image using cv2.imread("filename.jpg").

### Step3:
Convert the image into the given color transformation using cv2.cvtColor(image, cv2.BGR2YCrCb) and similarly for other color formats.

### Step4:
Split and merge the image using cv2.split(hsv) and cv2.merge([h,s,v]).

### Step5:
Output the image using cv2.imshow("OUTPUT", image).

## Program:

# Developed By:PRAKASH M
# Register Number:212222100035
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('ben.jpg')
cv2.imshow('212222100035_PRAKASH',houseImage)
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
houseHSVImage = cv2.imread('ben.jpeg')
cv2.imshow('212222100035_PRAKASH',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()


```




# iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('ben.jpg')
cv2.imshow('212222100035_PRAKASH',houseImage)
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
image = cv2.imread('benten.jpg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('212222100035_PRAKASH',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()

```



# v) Split and merge HSV Image

```
import cv2
image = cv2.imread('ben.jpg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('212222100035_PRAKASH',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow()
```
## Output:
### i) BGR and RGB to HSV and GRAY
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/8dc7d6d1-cda7-489b-a30a-20bf8884e6f5)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/56c2a85c-0852-4952-ac22-8a85f7df56c4)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/b398319b-a020-4d12-b831-6b09058a7bbe)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/30553013-8505-4c7c-8d1e-750499781408)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/e46ae5c9-75ca-41ec-adf3-d9fdf3797818)

### ii) HSV to RGB and BGR
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/d30831b0-cb17-4762-a65f-90611676e141)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/2452f0b9-620d-44c3-a6ed-2dac09e60282)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/0c3a524a-8628-40e6-be47-194c0bd83916)

### iii) RGB and BGR to YCrCb
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/6908a373-9728-47d8-8ebe-077473795119)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/f7a90b01-8faa-4a22-8c16-690fac39db17)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/cf2c5e47-f67d-470d-8721-6f6a99fd695f)

### iv) Split and merge RGB Image
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/f006398f-385a-46d0-833f-0921ca7e8b0a)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/3133c54d-534c-4231-bdae-2fa78c409df8)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/1b538ba5-bb8a-483c-a713-481ebf5e4d10)
![image](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/d9fcbb78-7172-4ade-97c8-d92143e7acb2)

### v) Split and merge HSV Image
<img width="722" alt="image" src="https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/e4575414-10fe-48ea-b9f4-f1729f3155a9">
<img width="719" alt="image" src="https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/a24de93e-a892-4c6e-8a8d-bd77dcb32b8b">

![im53](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/944beb07-2ed0-49cd-a0c4-96b88ad38d39)

![im54](https://github.com/Prakashmathi2004/COLOR-CONVERSION/assets/118350045/dcdeec7f-1285-495b-9daf-3754c5326fde)




## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
