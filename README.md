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
Once you done spliting, press train model on the top right (under dataset catorgery if you somehow not in here). Then select custom Tranining rather than instant model so we can try it later on our local device. Then, just click continue without doing anything until you see the "This version doesn't have a model.", then hit custom train. Select Roboflow 3.0 Object Detection -> select fast -> 
Train from Public Checkpoint -> start training. Then you can take a coffe break and come back since it takes some times depend on your amount of data.

## Step 8
When your model training is done, click model catogory on the left, then click the name of your model (the one beside robotflow instant). Congradulation, you just trained your own AI model on robotflow. You can try it out by find some other gokart image online to test out your model is working well or not.

# Step 9
Great we got a model working online. Let's try to run it on local computer and see if it can do the same thing. To do so, you need 3 things: 1. private api key belongs to the workspace 2. the model url 3. some python code

To get the api key, checkout the dark color bar on the left, you should see a gear icon, and your account icon should be down there. If you click the gear icon, it should pop up Workspace Setting. Select API keys, copy the private api somewhere then you can use it later. Then, go back to your projects, select your the model you trained. Copy down the Model URL somewhere for later use.

Then, clone this repo and open test.py. Change line 10 where it says model id to the Model URL you copyed. Lastly, change the image file to the correct image name.

# Step 10
Install the lib using:
```
pip install inference
```
then run it with your api key:
```
export ROBOFLOW_API_KEY="your-api-key"
```
then
```
python test.py
```
If the program runs properly, it should pop up an image with boxed target. If not, please paste the error from terminal and ask my best friend chatgpt for guidence XD. 

Congratulations! You’ve completed the training and deployment of your model on Roboflow. There’s a lot of potential for AI training on Roboflow — you can explore different functionalities such as workflows or experiment with various models to achieve your desired results. You can also download and use models shared by others right away.

Anyway, I hope you enjoyed this walkthrough, and I’m looking forward to seeing you showcase more in Triton AI!
