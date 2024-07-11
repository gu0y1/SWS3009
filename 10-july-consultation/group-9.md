---
description: Project Retrieval Robot
---

# Group 9

**Objective:** Develop a robot that can follow a person, recognize specific projects, and retrieve them using a tuned IMU and deep learning techniques.

#### Deep Learning:

1. **Person Following:**
   * **Task:** Implement a model that enables the robot to follow a person accurately.
   * **Technique:** Utilize deep learning algorithms to identify and track the person.
2. **Project Recognition:**
   * **Task:** Recognize specific projects using visual data.
   * **Implementation:**
     * Use anchor points with printed labels for project identification.
     * Train a model to recognize these labels and distinguish different projects.
3. **Gesture Recognition:**
   * **Requirement:** Implement gesture recognition by Friday.
   * **Technique:** Train a deep learning model to recognize hand gestures and interpret commands.

#### Robotics and Hardware:

1. **IMU Tuning:**
   * **Algorithm:** Use the Kalman Filter Algorithm to tune the IMU for better accuracy.
   * **Anchor Points:** Utilize anchor points with printed labels to assist in localization and tuning.
2. **Mechanism for Retrieval:**
   * **Task:** Design a mechanism to push or retrieve projects.
   * **Design Considerations:**
     * Ensure the mechanism can handle different types of projects securely.
     * Focus on creating a reliable and efficient retrieval system.

#### Implementation Steps:

1. **Deep Learning Development:**
   * **Person Following:** Collect and annotate a dataset for person tracking.
   * **Project Recognition:** Create and label a dataset of projects with anchor points.
   * **Gesture Recognition:** Gather and annotate data for gesture recognition and train the model.
2. **IMU Tuning:**
   * **Kalman Filter Implementation:** Develop and test the Kalman Filter for IMU tuning.
   * **Anchor Points:** Place and label anchor points in the environment to assist with IMU tuning and localization.
3. **Mechanism Design:**
   * **Prototype Development:** Design and build a prototype for the project retrieval mechanism.
   * **Testing:** Test the mechanism's ability to push and retrieve various projects.

#### Next Steps for Students:

1. **Deep Learning Tasks:**
   * **Dataset Preparation:** Collect and label data for person following, project recognition, and gesture recognition.
   * **Model Training:** Train models for each task and validate their performance.
2. **IMU Tuning:**
   * **Kalman Filter:** Implement the Kalman Filter for IMU tuning and validate its accuracy using anchor points.
   * **Localization:** Test the system's localization accuracy with the tuned IMU.
3. **Mechanism Development:**
   * **Design:** Develop a reliable mechanism for pushing and retrieving projects.
   * **Integration:** Integrate the mechanism with the robot's control system and test its performance.

#### Final Considerations:

* **System Integration:** Ensure seamless integration of deep learning models, IMU tuning, and the retrieval mechanism.
* **Testing and Iteration:** Conduct thorough testing and iterate on the design based on feedback to improve accuracy and reliability.
* **User Interaction:** Focus on creating an intuitive and user-friendly system for person following and gesture recognition.

#### Summary:

* Use the Kalman Filter Algorithm to tune the IMU for better localization.
* Implement deep learning models for person following, project recognition, and gesture recognition.
* Design and build a mechanism to push or retrieve projects, ensuring seamless integration and reliable performance.
