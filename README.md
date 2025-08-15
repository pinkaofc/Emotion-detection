🎭 Real-Time Emotion Detection

A Python application that uses OpenCV and DeepFace to detect human emotions in real-time through a webcam feed.
It identifies faces using Haar Cascade classifiers and predicts the dominant emotion for each detected face.

🚀 Features

Real-time face detection using OpenCV Haar Cascade.

Emotion prediction using DeepFace with a pre-trained deep learning model.

Supports multiple emotions like: happy, sad, angry, surprise, neutral, and more.

Works on live webcam feed.

Easy to run and modify.

📂 Project Structure
.
├── emotion.py                         # Main script for emotion detection
├── requirements.txt                   # Python dependencies
├── haarcascade_frontalface_default.xml # Haar Cascade file for face detection
└── README.md                          # Project documentation

🛠 Requirements

All dependencies are listed in requirements.txt
.

Key libraries:

opencv-python

deepface

tensorflow

keras

numpy, pandas

flask (optional, for web deployment)

📥 Installation

Clone the repository

git clone https://github.com/your-username/real-time-emotion-detection.git
cd real-time-emotion-detection


Install dependencies

pip install -r requirements.txt


Ensure Haar Cascade file is present
The file haarcascade_frontalface_default.xml must be in the same directory as emotion.py or inside the OpenCV data/haarcascades folder.

▶️ Usage

Run the script:

python emotion.py


The webcam will open.

Detected faces will be outlined with a red rectangle.

The predicted emotion will be displayed above each face.

Press q to quit.

📸 Example Output

When running, the program will look something like this:

[ Webcam feed ]
[ Face detected ] -> "happy"
[ Face detected ] -> "neutral"

📌 Notes

This script uses your default webcam (VideoCapture(0)).

Ensure your environment supports TensorFlow/DeepFace and has access to a GPU for faster inference.

For higher accuracy, run in good lighting conditions.

📄 License

This project is licensed under the MIT License – feel free to modify and use it.

💡 Future Improvements

Deploy as a web app using Flask.

Add support for image/video file input.

Integrate with AWS Rekognition for cloud-based emotion analysis.
