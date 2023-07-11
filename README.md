
# Metaverse_Classroom
Built a realistic classroom using metaverse that  mimics the original classroom. Through this project, we have created a virtual classroom model along with an avatar that is animated to move through the classroom and can change perspectives as needed.

Objectives
```
To create a virtual classroom/school world accessible through the PC or VR headsets.  
To incorporates features such as simulations, projections, holograms, etc.  
To implement methods for multiple users to log in and interact with others in real-time within the environment.  
To implement monitoring systems to watch the students and assist teachers in classroom activities.  
```

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

If you testing on a different processor a GPU consider making a pull request to add the FPS obtained on that processor.

## Demo

| <img src="https://github.com/Alleny244/Metaverse_Classroom/assets/56961826/baa58e66-792a-43aa-9c0b-a529272d25fb"  width="300" height="300"> | <img src="https://github.com/Alleny244/Metaverse_Classroom/assets/56961826/aa3bc7d1-5a1a-40a6-bfa7-36733158c2cd"  width="300" height="300">                        |
| ----------------------------------- | ----------------------------------- |
| <img src="https://github.com/Alleny244/Metaverse_Classroom/assets/56961826/4e987197-3a94-432c-beb8-3ff22d336917"  width="300" height="300"> | <img src="https://github.com/Alleny244/Metaverse_Classroom/assets/56961826/baa58e66-792a-43aa-9c0b-a529272d25fb"  width="300" height="300">  |


  
## Collaborators
  | |  |  |  |  |
  | ------------- | ------------- | ------------- | ------------- | ------------- |
  | Allen Y| [GitHub](https://github.com/Alleny244) | 
   |      Alvin Antony  K | [Github](https://github.com/alvinantonyk) |
  |      Divina Josy | [Github](https://github.com/diina7) |
  |    Gifty Treesa Iju   | [GitHub](https://github.com/Giffff) | 



## Contributing

If you have any other ideas or do any step of to do consider making a pull request . Please update the README as well in the pull request.


