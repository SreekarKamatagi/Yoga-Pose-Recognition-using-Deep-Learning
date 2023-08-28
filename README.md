# Yoga-Pose-Recognition-using-Deep-Learning
A Web Application using Tensorflow in Backend and ReactJS in Frontend which guides the Users to practice, perform and rectify their improper postures using Deep Learning.
This Project was successfully published in the 2nd International Conference on Sustainable Computing and Data Communication Systems which was held in Erode, India hosted by IEEE.
The proposed work is divided into two phases, the Backend phase and Frontend phase.
In the Backend Phase the process is broken down into three major steps:
1) Creating a Human Body Instance for developing a Pose Recognition Model: In this, a Human Body skeleton is recognised by defining seventeen body keypoints in our body.
  0 	Nose 	              9 	Left Wrist 
  1 	Left Eye 	         10 	Right Wrist 
  2 	Right Eye 	       11 	Left Hip 
  3 	Left Ear 	         12 	Right Hip 
  4 	Right Ear 	       13 	Left Knee 
  5 	Left Shoulder 	   14 	Right Knee 
  6 	Right Shoulder 	   15 	Left Ankle 
  7 	Left Elbow 	       16 	Right Ankle 
  8 	Right Elbow
2) Creating a Pose Detection Model based on Person's scores using TensorFlow Lite Model: Here we are using the help of Movenet Model available in the official website of Tensorflow from where we can predict the visibility scores of all input images taken for seven Yoga Poses (1) Chair Pose, 2) Cobra Pose, 3) Dog Pose, 4) Shoulder Stand, 5) Triangle Pose, 6) Tree Pose, 7) Warrior Pose. Some necessary Image Cropping processes are done to enhance the efficiency of Recognition model.
3) Finding Range and Accuracy of each Yoga Pose: In the final step, we are using the Euclidean Distance Metric to help the Model sense a pattern of distances from all bofy parts to the Pose Center (which changes based on Center of Gravity of each Yoga Pose).
Now in the Frontend Phase we use ReactJS with Tensorflow js extension in the backend to create a web application which is easy to understand, after designing the Home Page and Pose Recognition page with utilities to improve UI experience.
