# TV_time_tracking_face_recognition

Wonder how much time we spend watching TV!
This project aims to build a tracker that measures the amount of time spent in front of the TV of specifically registered individuals in a household.
Developed on top of [Keras-OpenFace](https://github.com/iwantooxxoox/Keras-OpenFace), a project converting OpenFace from its original Torch implementation to a Keras version, 
this tracker recognizes the faces of registered family members who are facing a camera mounted on the TV and enable a timer.
When TV is on and whenever the tracker recognizes faces looking toward it, an individual timer gets enabled for that person(s).    

## [TV_time_tracking_face_recognition Version 3 (TTT_v3)](https://github.com/sungsujaing/TV_time_tracking_face_recognition/blob/master/TV_time_tracking_face_recognition_v3.ipynb)
Multi-face recognition on a video: based on the images stored in the database, TTT_v3 successfully recognizes registered faces on a video with great accuracy. In TTT_v3, the blue bounding boxes (for unregistered faces and falsely-detected faces) are not tracked as they are not needed for the purpose of the developing TV time tracker. Compared to TTT_v2, most helper functions were re-written for clarity and efficiency.

### TTT_v3 video face recognition example
<p align="center">
<img src="Readme_images/TTT_v3_sean_test.gif" width="650"></p>
</p>

<p align="center">
<img src="Readme_images/TTT_v3_sean_test_result.png" width="650"></p>
</p>

---
### Upcoming for future TTT
* the model will be implemented to a real-time module. 
* the device will be mounted on a TV for a demo!
---
## [TV_time_tracking_face_recognition Version 2 (TTT_v2)](https://github.com/sungsujaing/TV_time_tracking_face_recognition/blob/master/TV_time_tracking_face_recognition_v2.ipynb)
Multi-face recognition on an image: based on the images stored in the database, TTT_v2 successfully recognizes registered faces on an image with great accuracy. TTT_v2 also differentiates registered faces from unregistered ones.

### TTT_v2 summary
<p align="center">
<img src="Readme_images/TTT_v2_summary.png" width="700"></p>
</p>

### Differentiating registered (red) from unregistered (blue) faces
<p align="center">
<img src="Readme_images/TTT_v2_not_registered_example.png" width="500"></p>
</p>

## [TV_time_tracking_face_recognition Version 1 (TTT_v1)](https://github.com/sungsujaing/TV_time_tracking_face_recognition/blob/master/TV_time_tracking_face_recognition_v1.ipynb)
Single face recognition on an image: based on the images registered in the database, TTT_v1 successfully recognize the face of the same person.

### Database registration process
<p align="center">
<img src="Readme_images/TTT_v1_database_registration.png" width="700"></p>
</p>

### Face recognition example
<p align="center">
<img src="Readme_images/TTT_v1_face_recognition_example.png" width="500"></p>
</p>

### Limitation of TTT_v1: unable to detect/recognize multiple faces
<p align="center">
<img src="Readme_images/TTT_v1_face_recognition_fail_example.png" width="500"></p>
</p>
