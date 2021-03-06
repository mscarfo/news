# Project ideas

## Help software heritage by writing a new lister for your favorite forge

https://www.softwareheritage.org/2017/03/24/list-the-content-of-your-favorite-forge-in-just-a-few-steps/


## Forensic database of images

In this project, you will learn to apply machine learning techniques to images. OpenCV is the recommended tool and Python is the recommended programming language. You may also use other machine learning models, such as deep learning if you can get high performance. The project has two milestone objectives – image classification and object detection.

    Problem 1 – Image Classification

You will be given a dataset - “body” which contains annotated sub-images of body parts, including ear, eye, hair, head, left foot, and mouth. These labeled sub-images will serve as the ground truth. The problem is as follows, can you provide a machine learning algorithm to automatically label new sub-images? Here are a few tips using OpenCV. For each image, you will be able to extract keypoints representing high-level features. Read through ORB (Oriented FAST and Rotated BRIEF) and Feature Matching to get some ideas. Then you need to try out classifying the sub-images based on the detected keypoints. Note that each image may have a different number of keypoints and different keypoints may represent different features. Binary classification, for instance, left foot vs. eye AND left foot vs. others, are desired. Ten-fold cross-validation could be used to measure and improve the model performance. Finally, you need to write up the algorithm, chosen parameters, and classification performance (i.e., mean and std of accuracy).

    Problem 2 – Object Detection

In the Problem 1, you are given the annotated sub-images. The harder problem would be, how can you detect the body parts from the full images, which may contain multiple body parts? Note that when you detect left foot, only some of the full images contain this body part. Same with the other body parts.

This problem contains two image datasets. One is exactly the one used in Problem 1, another is the dataset of the full images - “images”. Moreover, the two datasets are connected via the file “tags.csv”. In the CSV file, the column “ID” contains the sub-images’ names, the column “tag” gives the tag of each sub-image, and the column “Image” tells which full image the sub-image is from. There are several ideas to solve this problem. One idea is that you can split the full image into several (i.e., 3 * 4) sub-images and classify the sub-images based on the model you train when solving Problem 1. Another idea is that the full image should contain left foot if it contains sufficiently many similar keypoints from the annotated left foot sub-images.

     

#  A general list
http://www.ece.rutgers.edu/~marsic/books/SE/projects/

http://nevonprojects.com/web-based-project-ideas-topics/
