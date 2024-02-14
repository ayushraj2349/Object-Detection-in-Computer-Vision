[![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org) 
[![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable) 
[![pytorch](https://img.shields.io/badge/PyTorch-2.1.0-EE4C2C.svg?style=flat&logo=pytorch)](https://pytorch.org)

# Object Detection in Computer Vision

|![Object Detection](https://miro.medium.com/v2/resize:fit:828/format:webp/1*IrptRDRG8IL9o-55BKjbLA.png)|
|:--:|
|Object Detection|


## Helmet Detection by using *Faster R-CNN* and *YOLOv8* Models

## This Repository contains 3 Project Works on Object Detection:

## ! If any of the files is showing any type of error, you can also use this [Drive Link](https://drive.google.com/drive/folders/1g-1384mGscvzo8tQrMRi3TiSOdwZspVM?usp=sharing) given here. 

[Dataset used for these Projects (Kaggle)](https://www.kaggle.com/datasets/andrewmvd/hard-hat-detection)

This dataset, contains 5000 images with bounding box annotations in the PASCAL VOC format for these 3 classes:

They're [helmet, head & person], but mainly to predict helmet because the data is heavily imbalanced.

|![labels](https://github.com/ayushraj2349/Object-Detection-in-Computer-Vision/assets/97942801/28fcb9be-bcc0-4277-abd7-bd5bd015837c)|
|:--:|
|As you can see from the histogram above, **almost 75% of the occurences in the Dataset is of helmet class.**|

## We've partitioned the Dataset into Train, Val & Test Splits in Proportion of 8:1:1.


# Project 1 
We've used pre-trained **Faster R-CNN Model with Resnet50** backbone fine-tuned on this Dataset's Train Split.

Then we evaluated the model on the test split. The Results are like : 

|![download (1)](https://github.com/ayushraj2349/Object-Detection-in-Computer-Vision/assets/97942801/179fa479-b8d6-4fd4-b874-15f63525e7e9)|
|:--:|
|***Faster R-CNN***|
|Predictions on a random image of the test dataset.|
|Green & Yellow Boxes represent the actual & predicted boxes respectively.|
|The results are quite good, although the model also predicted some redundant boxes.|

We've used the standard **mAP@0.5** Performance Metric (where 0.5 denotes the IoU Threshold Value taken) for evaluation.

We've also calculated the Precision & Recall Values for each class though.

## mAP@0.5 Value
![Static Badge](https://img.shields.io/badge/mAP__Faster_R--CNN-25.34%25-red)

# Project 2
We've used the SOTA Model **YOLOv8** (Medium Version) fine-tuned on the same dataset.

And the Results & the speed of inference were quite Promising. Have a look :  

|![hard_hat_workers989](https://github.com/ayushraj2349/Object-Detection-in-Computer-Vision/assets/97942801/3a03ad57-1a9e-4d82-8b05-7f78663a077b)|
|:--:|
|***YOLOv8***|
|Predictions on a random image of the test dataset.|
|Not only the model was able to predict **helmet** class accurately with good confidence, it was able to predict **head** class well. Again, some redundant boxes.|

Here also we've used the **mAP@0.5** Performance Metric for evaluation & comparision b/w the 2 Models.  

Here again also, we've calculated the Precision & Recall Values for each class.  

## mAP@0.5 Value
![Static Badge](https://img.shields.io/badge/mAP__YOLOv8-63.40%25-brightgreen)

# Comparing the two Models
**YOLOv8**, the new State of the Art Model is quite accurate & fast comparative to the conventional models used for Object Detection Models, like here we used **Faster R-CNN**. And the results are quite astonishing. 

   
While the Faster R-CNN struggled a bit giving a quite low *mAP @0.5* value as **"25.34%"**, on the other hand, YOLOv8 totally outperformed the former model by giving the same value as **"63.40%"**.  

Also due to its rapid processing speed, it takes around only *10ms* on an avg. for an image prediction while the latter one takes around *142ms* for the same. 

**Almost 15x times faster.**  

So, It easily surpasses the criteria of **24fps** for a model to be run on Video. **(YOLOv8 FPS = 83FPS)**

```diff
- It can be used conveniently for REAL-TIME Detection & this leads to many Real-World Applications.
```

# Project 3


https://github.com/ayushraj2349/Object-Detection-in-Computer-Vision/assets/97942801/dcbdcfc9-0049-4d11-841f-4b542a9db88c


## A smaller yet powerful Project build using YOLOv8 to showcase one out of many real-world applications.

## This tool simply plots the bounding boxes of Helmets without confidence score (else it will become clumsy, just to look clean) and displays the current count of Helmets in the videos.

This tool can be very useful for real-time video surveillance, traffic monitoring, and autonomous systems.

You can also use more features like ability to track objects, maintain identities, handle occlusions and noise in this tool.

For giving you just a simple example, ***Traffic Camera*** - this tool can be implemented in city surveillance cameras to give an automated estimate of how well are the traffic rules being followed (if helmets are mandatory).



# Authors - Ayush Raj & Vikash Kumar Thakur

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

**Ayush Raj**  

[![gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](ayushraj2349@gmail.com)
[![image](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ayush-r-bb88b8236/)
[![github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ayushraj2349)
[![kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)](https://www.kaggle.com/ayushraj2349)
[![medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@ayushraj2349)

**Vikash Kumar Thakur**

[![gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](vkthakur082002@gmail.com)
[![image](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](linkedin.com/in/vkt08)
[![github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/vkt08)
[![kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)](https://www.kaggle.com/vikashkumarthakur08)
[![medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@vkt08)
