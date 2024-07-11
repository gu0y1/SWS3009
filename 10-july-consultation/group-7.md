---
description: Smart Guide Dog Companion
---

# Group 7

**Project Objective:** The project aims to develop a Smart Guide Dog Companion to assist visually impaired individuals by providing navigation, emotional support, and daily living assistance through advanced technologies.

**Key Features:**

1. **Navigation Module:**
   * Utilizes sensors to detect the environment and plan safe routes.
   * Employs path planning and obstacle avoidance algorithms.
   * Integrates voice interaction for navigation commands.
2. **Emotional Support:**
   * Analyzes voice, behavior, and facial expressions for emotional recognition.
   * Provides predefined comfort phrases and connects to remote psychological consultations if needed.
3. **Daily Living Assistance:**
   * Manages medication reminders and confirmations.
   * Integrates with smart home controls for lighting, temperature, and security.

**Deep Learning Components:**

1. **Data Collection:**
   * Obstacle data from various road scenarios.
   * Body language and facial recognition data using datasets like FER-2013, AffectNet, and CK+.
2. **Model Selection:**
   * Uses Wav2Vec 2.0 or Whisper for audio analysis, OpenPose or MediaPipe for body language detection, and DeepFace for facial expression recognition.
   * Combines models using frameworks like Hugging Face’s Transformers or DeepMind's Perceiver.
3. **Input Preprocessing:**
   * Converts audio to spectrograms, normalizes signals, and segments audio.
   * Extracts and normalizes keypoints for body and facial features.
   * Tokenizes and encodes text, removing noise and handling stop words.
4. **Result Processing:**
   * Outputs probabilistic scores for detected emotions and assesses their severity.
   * Generates comforting words using TTS models like Tacotron or WaveNet.
   * Integrates with real-time communication tools for remote psychological support.

**Robotics Components:**

1. **System Implementation:**
   * The model is implemented on a smart car with a camera for computer vision, ultrasonic sensors for obstacle detection, and a microphone for voice commands.
2. **Autonomy:**
   * The car navigates autonomously using navigation algorithms and communicates via a web interface for real-time monitoring and decision-making.

**Teacher's Comments:**

1. **Deep Learning:**
   * Focus on obstacle avoidance using YOLO and consider video analysis or map design instead of SLAM for localization.
   * Implement a smaller version of the environment using Navilens.
2. **Robotics:**
   * Increase human-robot interaction to enhance user experience.

We would like to see the juction detection in next meeting. Please give a prototype of physical condition between the robot and the blind people.&#x20;
