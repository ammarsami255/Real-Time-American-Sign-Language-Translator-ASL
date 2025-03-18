# Real-Time-American-Sign-Language-Translator-ASL
Hand Gesture Recognition using Mediapipe and Machine Learning

This project uses OpenCV, MediaPipe, and a trained machine-learning model to recognize hand gestures and classify them as letters (A-Z) and digits (0-9). The application captures real-time video input, processes hand landmarks using MediaPipe, and predicts the corresponding character using a pre-trained model.

Requirements

Before running the project, ensure you have the following dependencies installed:

pip install opencv-python mediapipe numpy pickle

Usage

Load Model: The script loads a pre-trained model from model.p.

Capture Video: It uses OpenCV to capture frames from the webcam.

Hand Detection: MediaPipe detects and processes hand landmarks.

Feature Extraction: The landmark positions are extracted and normalized.

Prediction: The trained model predicts the corresponding character.

Display Output: The predicted character is displayed on the screen.

Running the Code

Run the following command in your terminal:

python inference_classifier.py or py inference_classifier.py

Press q or Esc to exit the application.

File Structure

main.py: The main script for hand gesture recognition.

model.p: Pickle file containing the trained model.

README.md: Documentation for the project.

Expected Output

The webcam feed will display a bounding box around the detected hand.

The recognized character will be displayed above the hand in the frame.

Troubleshooting

If the webcam does not turn on, ensure it is properly connected.

If detection is inaccurate, try improving the lighting conditions.

Ensure the model.p file is present in the project directory.

Future Enhancements

Improve model accuracy with more training data.

Extend the model to recognize hand gestures for sign language.

Implement a real-time prediction smoothing algorithm.

License

This project is open-source and available for further development and contributions.
