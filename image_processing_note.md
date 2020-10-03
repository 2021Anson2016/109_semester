# 109上 影像處理
###### tags: `專業`


# 0918

## Interpolation
1. Nearest-Neighbor：又稱為zero order interpolation，使用一個最近的相鄰像素。
2. Bilinear：又稱為first order interpolation，使用四個最近的相鄰像素。
3. Bicubic：又稱為second order interpolation，使用十六個最近的相鄰像素。

---

1. Nearest Neighbor Interpolation
介紹：
    顧名思義，此演算法是利用最近的相鄰點的值來填入。如下圖，新(右)圖的P'點因為最相鄰原(左)圖的P點，所以就將P點的值填入P'。


2. 介紹：
    Bilinear Interpolation會利用最近相鄰的四個點依相鄰的(比例)程度來填入。如下圖，新(右)圖的P'點因為最相鄰原(左)圖的P(1,1),P(1,2),P(2,1),P(2,2)四點，所以就將此四點的值依比例填入P'。
公式：P'(x,y)=(1-d)(1-d')P(1,1)+d(1-d')P(1,2)
       +d'(1-d)P(2,1)+d*d'*P(2,2)


3. Bicubic Interpolation
介紹：
    Bilinear Interpolation會利用最近相鄰的十六個點來填入。
    
    
![](https://i.imgur.com/tRZmuX5.png)

### ref
http://yzu1022cs362s1001549.blogspot.com/2014/03/opencv.html


## openCV autocomplete on VScode

https://marketplace.visualstudio.com/items?itemName=did1335.opencv-intellisense

* Start
* View-->Command Palatte... OpenCV Intellisense
https://github.com/OpencvIntellisense/opencv-intellisense


* You can use cv2.__file__ to get path to the module and then use os.path to resolve symlinks and do some path manipulation.




# 0922

### Image Enhancement in the Spatial Domain
https://blog.xuite.net/viplab/blog/307263602-Image+Enhancement+in+the+Spatial+Domain