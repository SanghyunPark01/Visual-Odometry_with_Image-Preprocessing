# Visual-Odometry_with_Image-Preprocessing
ORB Feature기반 Visual Odometry 에서 이미지 전처리 과정을 통해 얻은 Odometry와 Original Odometry 비교

# Image Filter
* HPF  
* HPF-임계값 적용
* LPF-AVG
* LPF-Gaussian Filter
* LPF-Median Filter
* LPF-Bilateral Filter

# Test  
**Green : Truth**

## Test1
Feature : 1500  
* Original
<p align="Left"><img src="img/1500_O.png" width="400px"></p>

* HPF(Left) / HPF-임계값 적용(Right)  

|HPF|HPF-임계값적용|
|:--:|:--:|
|<p align="Left"><img src="img/1500_HPF.png" width="400px"></p> | <p align="Left"><img src="img/1500_HPF_T.png" width="400px"></p>|  

* LPF-AVG(Left) / LPF-Gaussian Filter(Right)

|LPF-Average|LPF-Gaussian filter|
|:--:|:--:|
|<p align="Left"><img src="img/1500_AVG.png" width="400px"></p> | <p align="Left"><img src="img/1500_Gaussian.png" width="400px"></p>|  
  
* LPF-Median Filter(Left) / LPF-Bilateral Filter(Right)

|LPF-Median Filter|LPF-Bilateral Filter|
|:--:|:--:|
|<p align="Left"><img src="img/1500_Median.png" width="400px"></p> | <p align="Left"><img src="img/1500_Bilateral.png" width="400px"></p>|  

## Test2
Feature : 4000  
* Original
<p align="Left"><img src="img/4000_O.png" width="400px"></p>

* HPF(Left) / HPF-임계값 적용(Right)  

|HPF|HPF-임계값적용|
|:--:|:--:|
|<p align="Left"><img src="img/4000_HPF.png" width="400px"></p> | <p align="Left"><img src="img/4000_HPF_T.png" width="400px"></p>|  

* LPF-AVG(Left) / LPF-Gaussian Filter(Right)

|LPF-Average|LPF-Gaussian filter|
|:--:|:--:|
|<p align="Left"><img src="img/4000_AVG.png" width="400px"></p> | <p align="Left"><img src="img/4000_Gaussian.png" width="400px"></p>|  
  
* LPF-Median Filter(Left) / LPF-Bilateral Filter(Right)

|LPF-Median Filter|LPF-Bilateral Filter|
|:--:|:--:|
|<p align="Left"><img src="img/4000_Median.png" width="400px"></p> | <p align="Left"><img src="img/4000_Bilateral.png" width="400px"></p>|  

# Result
## Test1
<p align="Left"><img src="img/res1.jpg" width="800px"></p>

## Test2
<p align="Left"><img src="img/res2.jpg" width="800px"></p>

# Conclusion
* Feature 갯수가 적을 때는 이미지 전처리를 하지 않고 Odometry를 추정하는 것이 더 성능이 좋았다.
* Feature 갯수가 많을 때는 Gaussian 필터를 적용해 전처리를 한 후 Odometry를 추정하는 것이 더 성능이 좋았다.