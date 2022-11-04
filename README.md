# Image Denoising Using AutoEncoders

![N|Solid](https://imgs.search.brave.com/Rm6XcByPNCXMzbD3WNGbVs01VxGEqB2Y_2TsNi8wdSc/rs:fit:2739:225:1/g:ce/aHR0cHM6Ly90c2Uy/Lm1tLmJpbmcubmV0/L3RoP2lkPU9JUC5Z/OVMxQ09jYld6aGp6/aTdOZ2dzZ3B3SGFC/UyZwaWQ9QXBp)



### Abstract

With the explosion in the number of digital images taken every day, the demand for more accurate and visually pleasing images is increasing. However, the images captured by modern cameras are inevitably degraded by noise, which leads to deteriorated visual image quality. Therefore, work is required to reduce noise without losing image features (edges, corners, and other sharp structures). So far, researchers have already proposed various methods for decreasing noise. Each method has its own advantages and disadvantages. In this paper, we summarize some important research in the field of image denoising. First, we give the formulation of the image denoising problem, and then we present several image denoising techniques. In addition, we discuss the characteristics of these techniques. Finally, we provide several promising directions for future research.





### Introduction

Owing to the influence of environment, transmission channel, and other factors, images are inevitably contaminated by noise during acquisition, compression, and transmission, leading to distortion and loss of image information. With the presence of noise, possible subsequent image processing tasks, such as video processing, image analysis, and tracking, are adversely affected. Therefore, image denoising plays an important role in modern image processing systems.

Image denoising is to remove noise from a noisy image, so as to restore the true image. However, since noise, edge, and texture are high frequency components, it is difficult to distinguish them in the process of denoising and the denoised images could inevitably lose some details. Overall, recovering meaningful information from noisy images in the process of noise removal to obtain high quality images is an important problem nowadays.

In fact, image denoising is a classic problem and has been studied for a long time. However, it remains a challenging and open task. The main reason for this is that from a mathematical perspective, image denoising is an inverse problem and its solution is not unique. In recent decades, great achievements have been made in the area of image denoising.


### AutoEncoders
Autoencoders are an unsupervised learning technique in which we leverage neural networks for the task of representation learning. Specifically, we'll design a neural network architecture such that we impose a bottleneck in the network which forces a compressed knowledge representation of the original input. If the input features were each independent of one another, this compression and subsequent reconstruction would be a very difficult task. However, if some sort of structure exists in the data (ie. correlations between input features), this structure can be learned and consequently leveraged when forcing the input through the network's bottleneck.

![N|Solid](https://imgs.search.brave.com/bWEXTVnR1YenBjG64A02nvY9iEAyto1a9E5UrzUGQUA/rs:fit:1200:1045:1/g:ce/aHR0cHM6Ly9kMW03/NXJxcWdpZHpxbi5j/bG91ZGZyb250Lm5l/dC93cC1kYXRhLzIw/MjAvMDQvMjkyMDI3/NDkvQmxvZ19pbmZv/XzI5LTA0LTIwMjAt/Ui0wMi0yMDQ4eDEw/NDUucG5n)







