# 💡 Driver's Drowsiness Detection using OpenCV-Python

🤔 Ever fallen asleep while driving alone? 

🤔 Ever saved yourself from any accident by waking up instantly and looking in the side mirror and thanking god, because you hadn't completed your sleep?

🤔 Did you ever think to have someone who will give you an alert while you are feeling drowsy?

😉 Python comes for the rescue here!

👉 I made a python script that will give an alert to the driver when the driver is feeling drowsy





## 💡 Implementation of the Logic

👉 Basically, I used the famous dlib library which can estimate the location of 68 coordinates (x, y) that map the facial points on a person’s face in real-time.<br>


**📸 Here is a Image to show 68 points on our face**

<img src="assets/68_landmark.jpeg" height=300px><br>

**🎥 Here is a GIF to show 68 points on Real face**

<img src="assets/68_points_gif.gif" height=300px><br>


👉 Then, I am calculating Eye Aspect Ratio (EAR) of Left Eye and Right Eye using Euclidean Distance between 3 pairs of different coordinates of both the eyes as seen in 68 Points landmark's image!

👉 Then, I set a threshold value, If EAR goes below that threshold point, It will alert the driver!

👉 Planning to integrate Lips Detection Algorithm also, to detect the driver is yawning or not!

👉 I am thinking to deploy it on a raspberry pi that will have an alarm attached to it so it can be really helpful to someone

   
**Note**: Incase, if you want to just detect the 68 points on Human face then run `face_landmark.py` file and You are good to go!😎

## 🙋‍♂️ Helpdesk

**If you face any problem like script not running in local environment or anything:** You can reach out to me at anytime on following platforms!


## ℹ References

The ideas presented in this repo came primarily from the Dlib library. The implementation here also took significant inspiration. The pretrained model used in this project came from the official Dlib website.

<ul type='square'>
  <li><strong>Davis.King - </strong><a href='https://github.com/davisking/dlib'>dlib C++ library</a></li>
  <li><strong>Italo José - </strong><a href='https://towardsdatascience.com/facial-mapping-landmarks-with-dlib-python-160abcf7d672'>Facial mapping (landmarks) with Dlib + python</a></li>
  <li><a href='https://pjreddie.com/darknet/yolo/'><strong>The official dlib </strong><a href='http://dlib.net/'>website</a></a></li>
</ul>


