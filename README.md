# insects_objectdetection
PoC for Object Detection for Insects

#Introduction
Object Detection has become available on Single Board Computers such as the Raspberry Pi 4 or Jetson Nano. Together with low code machine learning platforms such as EdgeImpulse, this has opened up new possibilities. 

Here a Object Detection model for insects is presented. With it, 5 classes of insects (bees, ants, earwigs, ladybirds and isopods) can be detected and counted. 

#Project Description
For each Class 10 images were collected. Preferably these are with a top view on a plain background. 
With the Data Augmentation notebook, these images are flipped and rotated to create 11 copies for each image. In total that means 120 images per class.

Then the images were uploaded to EdgeImpulse and a ObjecDetection model was trained.
The model was exported and a script was used on a Raspberry Pi 4 to run it.

This project is inspired by Shawn Hymel's course 'Computer Vision with Embedded Machine Learning' (see: https://www.coursera.org/learn/computer-vision-with-embedded-machine-learning) and also makes use of a Python script provided by EdgeImpulse.

#Future challenges
- Improve model quality. 
- Multi stage inferencing: combine Object Detection with Image Classification. 

