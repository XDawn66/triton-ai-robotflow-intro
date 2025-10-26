# triton-ai-robotflow-intro

## Intro
The goal of this repo is to help people who are new to ai model training to get an idea of the training process and provide a simple way to train, fine tune, and deploy your own ai model from sratch using robotflow.

## Step 1 
Go to the following [website](https://roboflow.com/) and login in. If you don't have one you can create a new one, recommanded to create your account using the school email so others can share projects to you more easily.

## Step 2
Once you are in, create your own work space (public plan). If you want to work with others, you can fill in their emails to invite them (optional). 

## Step 3
Once you inside your new project, please click project -> +project -> Object detection

## Step 4
Once you reach the point to upload data, you are at the very important point of the project. We all know that good quality data matter a lot when we try to get a good AI model, and the more high quaility data we put, the better the train will be. Therefore, please find a lot of images that has a clear gokart (since we are trition ai and we love evgokart) and put them into the upload data.

## Step 5
Nice, you got a bunch of imgs which is a good start. Unfortunately, AI are all babies in the beginning, and they don't know what is gokart. Now as their parent, you need to annoated all the images to tell AI what is what. Please go ahead and annoate your images by select label myself on the right, and draw boxes on the gokart and put label name as gokart. Click next image and label next, and once you finish, please exit thought the small left arrow on the top left. Then, hit add xx images to dataset on the top right.

It is indeed a lot of work once you get a lot of images, but later if you are more skilled. You can create your own AI model to help you to do labeling (classifcation model). 

## Step 6
Next, you need to click back to Dataset, and click images again and you should be in the labeling mode. On the top right, there's a purple button says train, and it means the picture will be used for training the model. However, training a AI model is often not enought, you need to provide them data to valid and test their prediction. Go and click on the train button and move at least 2 of your images to valid and at least 2 of your images to Test. This is called data split in AI training. Once you done, exit by clicking the same left arrow on the top left as you exit done labeling.

## Step 7
Once you done spliting, press train model on the top right (under dataset catorgery if you somehow not in here). Then select custom Tranining rather than instant model so we can try it later on our local device. Then, just click continue without doing anything until you see the "This version doesn't have a model.", then hit custom train. Select YOLOv11 -> select fast -> 
Train from Public Checkpoint -> start training. Then you can take a coffe break and come back since it take some times depend on your amount of data.

## Step 8


