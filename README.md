#EyeOnYou 
- Drowsiness Detection System
Overview
EyeOnYou is a real-time drowsiness detection system that monitors driver alertness by analyzing eye aspect ratio (EAR) through webcam input. If drowsiness is detected, an alarm is triggered to alert the driver.

Features
Real-time face and eye detection using dlib and OpenCV.
Eye aspect ratio (EAR) calculation to detect drowsiness.
Audio alert triggered when the user shows signs of drowsiness.
Adjustable detection threshold and frame count for custom sensitivity.
Requirements
Python 3.x
OpenCV
Dlib
Scipy
Imutils
Pygame
How to Run
Clone this repository:

bash
Copy code
git clone https://github.com/your-username/your-repo-name.git
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Download the shape_predictor_68_face_landmarks.dat model from here, extract it, and place it in the models directory.

Run the script:

bash
Copy code
python Drowsiness_Detection.py --show_video
Press q to stop the detection.

Customization
You can adjust the sensitivity of the detection by modifying the following parameters:

Threshold: Adjust the EAR threshold for drowsiness detection using the --threshold argument.
Frames: Set the number of consecutive frames for detection using the --frames argument.
Example
bash
Copy code
python Drowsiness_Detection.py --threshold 0.25 --frames 20 --show_video
License
This project is licensed under the MIT License.
