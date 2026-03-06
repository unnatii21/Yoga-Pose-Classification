# Yoga Pose Classification and Feedback System

A real-time yoga pose detection system using Computer Vision and Machine Learning that detects 5 yoga poses through a live webcam and provides instant joint-level feedback.

## Overview
This system helps users perform yoga poses correctly by detecting their pose in real time and telling them exactly which joints need adjustment and by how many degrees.

## Workflow
Input (Live Webcam) - MediaPipe Keypoint Extraction - Joint Angle Calculation - XGBoost Classification - Live Feedback on Screen

## Poses Detected
- Downdog
- Goddess
- Plank
- Tree
- Warrior2

## Tech Stack
- Python 3.10
- MediaPipe (body keypoint extraction)
- OpenCV (video processing)
- XGBoost (pose classification)
- scikit-learn (model evaluation)
- NumPy / Pandas (data handling)

## Results
| Metric | Score |
|--------|-------|
| Accuracy | 97.96% |
| F1 Score | 97.96% |
| Precision | 98.01% |
| Recall | 97.95% |
| R² Score | 0.9616 |
| RMSE | 0.2766 |

## Dataset
Kaggle Yoga Poses Dataset — 979 images across 5 pose classes

## Features
- Real time pose detection via webcam
- Joint angle computation at 10 key joints
- Instant feedback showing which joints are incorrect
- Shows exact degrees to increase or decrease per joint
- 97.96% classification accuracy

## Project Structure
- Yoga_Client.ipynb - main notebook with all code
- yoga_features.csv - extracted features from dataset
- xgb_model.pkl -  trained XGBoost model
- label_encoder.pkl - pose label encoder
- confusion_matrix.png -  model evaluation results
- requirements.txt - required libraries
- setup_instructions.md - how to run the project
