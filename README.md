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
Tech Stack:
```
Three.js
HTML,CSS
Blender
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
It is implemented in `face_detector.py` and is used for tracking eyes, mouth opening detection, head pose estimation, and face spoofing.

### Head pose estimation
`head_pose_estimation.py` is used for finding where the head is facing.

### FPS obtained

Functionality | On Intel i5
--- | ---
Head Pose Estimation | 8.5


If you testing on a different processor a GPU consider making a pull request to add the FPS obtained on that processor.


## Contributing

If you have any other ideas or do any step of to do consider making a pull request . Please update the README as well in the pull request.


