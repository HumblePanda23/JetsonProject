Amount of Materials

My project trained a dataset of pencils and it can identify the number of pencils in a picture.


## The Algorithm

First I downloaded a dataset of pencils and sorted through them into two groups. 4 or less pencils and 5 or more pencils. I trained the Jetson to recognize what pencils where, then how many there were. I followed Unit 6 as a guide to presenting the picture. I made my jetson follow the path into my many different folders until it had access to the pictures of the pencils. The jetson now recognizes how much of a pencil it is.

![pencil_output2](https://user-images.githubusercontent.com/108011081/183142437-cac5dbfd-0908-4460-b7f7-7a567d3561cf.jpg)


## Running this project

1. First, download an image of pencils that you want to identify then run the code below. But instead of 00156.jpg, replace it with the name of your picture. then where it says pencil_output3.jpg replace it with pencil_output4.jpg and so on.
2. 
3. imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt /home/nvidia/jetson-inference/python/training/classification/data/Jetson_Project/test/4_or_less_pencils/00156.jpg pencil_output3.jpg
4. 
5. Then open a new powershell and input the following code. Where it says pencil_output3, replace both of them with whatever you replaced pencil_output3 with in step 1.
6. You also need to replace "ethan" with whatever your hostusername is. then the picture will appear in your desktop with what percentage the pencil is.
7. 
8. scp nvidia@192.168.55.1:/home/nvidia/jetson-inference/python/training/classification/pencil_output3.jpg C:\Users\ethan\Desktop\pencil_output3.jpg

file:///C:/Users/ethan/Videos/2022-08-05%2015-10-24.mp4
(You might want to turn the volume up)
