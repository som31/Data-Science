# GestureRecognitionUsingDeepLearning
This project involves building a 3D Neural Network to correctly recognize hand gestures by a user to control a smart TV.

# Problem Statement:
The objective of this projects is to build a hand gesture recognition model that can be hosted on a camera installed in a smart TV that can understand 5 gestures.   
The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:  
-	Thumbs up:  Increase the volume  
-	Thumbs down: Decrease the volume  
-	Left swipe: 'Jump' backwards 10 seconds  
-	Right swipe: 'Jump' forward 10 seconds    
-	Stop: Pause the movie  

# About the Dataset: 
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.  
The videos have two types of dimensions - either 360x360 or 120x160 (depending on the webcam used to record the videos).  

### Data Source : https://drive.google.com/uc?id=1ehyrYBQ5rbQQe6yL4XbLWe3FMvuVUGiL

## References:

1.	Jeff Knup's blog: 'Yield' and Generator Functions  : https://jeffknupp.com/blog/2013/04/07/improve-your-python-yield-and-generators-explained/  

2.	Corey Schafer (YouTube video): Generator functions  : https://www.youtube.com/watch?v=bD05uGo_sVI 

3.	https://keras.io/preprocessing/image/  

4.	https://github.com/fchollet/deep-learning-models/releases/download/v0.6/mobilenet_1_0_224_tf_no_top.h5  

5.	http://www.image-net.org/  

6.	https://gist.github.com/yrevar/942d3a0ac09ec9e5eb3a  


