# Metaverse_Classroom
Built a realistic classroom using metaverse that  mimics the original classroom. 

Features:
```
Real world classroom experience.
Better monitoring systems.
Live student-student and student-teacher interaction. (To do)
Multiple avatars for teacher and students. (To do)
Less mental stress and feelings of isolation for students and teachers alike.
```

# Monitoring System-AI

Project to create an automated proctoring system where the user can be monitored automatically through the webcam and microphone. 
### Prerequisites

For vision:
```
Tensorflow>2
OpenCV
sklearn=0.19.1 # for face spoofing. 
The model used was trained with this version and does not support recent ones.
```

## Vision
 Head pose estimation to find where the person is looking.


### Face detection
Earlier, Dlib's frontal face HOG detector was used to find faces. However, it did not give very good results. In [face_detection](../../tree/master/face_detection) different face detection models are compared and OpenCV's DNN module provides best result and the results are present in [this article](https://towardsdatascience.com/face-detection-models-which-to-use-and-why-d263e82c302c?source=friends_link&sk=c9e2807cf216115d7bb5a9b827bb26f8).

It is implemented in `face_detector.py` and is used for tracking eyes, mouth opening detection, head pose estimation, and face spoofing.

An additional quantized model is also added for face detector as described in [Issue 14](https://github.com/vardanagarwal/Proctoring-AI/issues/14). This can be used by setting the parameter `quantized` as True when calling the `get_face_detector()`. On quick testing of face detector on my laptop the normal version gave ~17.5 FPS while the quantized version gave ~19.5 FPS. This would be especially useful when deploying on edge devices due to it being uint8 quantized.


### Head pose estimation
`head_pose_estimation.py` is used for finding where the head is facing. An explanation is provided in this [article](https://towardsdatascience.com/real-time-head-pose-estimation-in-python-e52db1bc606a?source=friends_link&sk=0bae01db2759930197bfd33777c9eaf4)

![head pose estimation](../../blob/master/gifs/4.gif)



### FPS obtained

Functionality | On Intel i5
--- | ---
Head Pose Estimation | 8.5


If you testing on a different processor a GPU consider making a pull request to add the FPS obtained on that processor.


## Contributing

If you have any other ideas or do any step of to do consider making a pull request . Please update the README as well in the pull request.


