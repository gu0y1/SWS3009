---
description: Police Chasing Robot
---

# Group 5

#### Objective:

* Develop a robot that can identify and chase a specific car based on a description, using deep learning techniques for object detection and tracking, and implement appropriate actions through robotics.

#### Deep Learning:

1. **Car Identification**:
   * **Description-Based Detection**: The system should identify a specific car based on given descriptions such as color (e.g., "a blue car") or make (e.g., "a Honda").
   * **Model Choice**: Utilize YOLO (You Only Look Once) for real-time object detection.
   * **Bounding Box Differentiation**: Highlight the identified car with a different colored bounding box for easy tracking.
2. **Trajectory Prediction**:
   * **Efficiency Improvement**: Implement trajectory prediction using RNN (Recurrent Neural Network) or transformer models to enhance the efficiency and accuracy of YOLO.
   * **Model Integration**: Integrate the trajectory prediction model with YOLO to anticipate the car's movement and adjust the tracking accordingly.
3. **Implementation Steps**:
   * **Dataset Collection**: Gather a dataset of car videos with various descriptions for training the YOLO model.
   * **Model Training**: Train YOLO for car detection and integrate RNN or transformer models for trajectory prediction.
   * **Testing**: Validate the system's accuracy and real-time performance with test videos.

#### Robotics:

1. **Action Proposal**:
   * **Possible Actions**: Determine the appropriate actions the robot should take upon identifying the target car, such as following the car or shooting (depending on the intended non-lethal design).
   * **Actuator Design**: Design actuators that can perform the proposed actions. Ensure the actuators are functional and safe.
2. **Camera Mobility**:
   * **Rotating and Tracking**: Equip the robot with a rotating camera capable of following the identified car.
   * **Autonomous Navigation**: Ensure the robot can move around autonomously while keeping the target car in view.
3. **Implementation Steps**:
   * **Camera System**: Develop a camera system that can rotate and follow the target car accurately.
   * **Actuation Mechanism**: Design and test actuators for the proposed actions, ensuring they work effectively with the camera system.
   * **Integration**: Ensure the camera and actuator systems work seamlessly with the deep learning model for real-time tracking and action execution.

#### Next Steps for Students:

1. **Deep Learning Tasks**:
   * **Data Collection**: Collect videos of cars with various descriptions.
   * **Model Training**: Train YOLO for car detection and integrate with RNN or transformer models for trajectory prediction.
   * **Model Validation**: Test the integrated model with video inputs to ensure accuracy and efficiency.
2. **Robotics Tasks**:
   * **Camera System**: Develop and test a rotating camera system that can follow the target car.
   * **Actuator Design**: Prototype actuators for proposed actions, such as following or shooting.
   * **System Integration**: Integrate the camera and actuator systems with the deep learning model for a cohesive and functional robot.
3. **Testing and Iteration**:
   * **System Testing**: Test the complete system in controlled environments to ensure it works as intended.
   * **Iterative Improvement**: Improve the system based on testing feedback, focusing on accuracy, reliability, and safety.

#### Final Considerations:

* **System Safety**: Ensure all actions performed by the robot are safe and non-lethal.
* **Real-Time Performance**: Focus on optimizing the system for real-time detection, tracking, and action execution.
* **Scalability**: Design the system to be scalable for different environments and scenarios.

#### Summary:

* Develop a deep learning model using YOLO and trajectory prediction techniques to identify and track a specific car.
* Design and implement actuators for proposed actions, ensuring they are integrated with the camera system.
* Focus on real-time performance, safety, and scalability to create an effective police chasing robot.
