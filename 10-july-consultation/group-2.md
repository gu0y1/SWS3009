---
description: Delivery Robot for Food Distribution to Animals
---

# Group 2

#### Hardware Considerations:

1. **Picking Mechanism**:
   * **Requirement**: The robot should be able to pick up various food items.
   * **Suggestions**:
     * Use a robotic arm equipped with a gripper or a magnet, depending on the type of food container.
     * Ensure the gripper can handle different shapes and sizes of food containers securely.
2. **Navigation and Localization**:
   * **Challenge**: Localization could be problematic in a dynamic environment.
   * **Suggestions**:
     * Implement QR codes on shelves and along the path to help with localization.
     * Use a straight-line path where possible to simplify navigation.
     * Utilize a 2D map for the robot to navigate, ensuring it can move efficiently within the mapped area.

#### Deep Learning:

1. **Object and Animal Identification**:
   * **Objective**: Develop a deep learning model to identify different food items and the specific animals.
   * **Prototypes**:
     * Train the model to recognize various food items.
     * Train the model to identify the xy coordinates of animals and their respective food items on the 2D map.
2. **Implementation Steps**:
   * **Prototype Development**: Build a prototype that can:
     * Identify food items using image recognition.
     * Locate animals based on the map coordinates and QR codes.

#### Operational Flow:

1. **Food Delivery Process**:
   * **Step 1**: Identify the food item to be delivered using the trained deep learning model.
   * **Step 2**: Pick up the food item using the robotic arm or magnet.
   * **Step 3**: Navigate to the animal’s location using QR codes for precise localization.
   * **Step 4**: Deliver the food item to the correct animal.

#### Next Steps for Students:

1. **Deep Learning Tasks**:
   * **Prototype Development**: Create a working prototype that can identify food items and determine their coordinates.
   * **Training**: Collect data and train the deep learning model for accurate identification.
2. **Robotics Tasks**:
   * **Pick-Up Mechanism**: Design and implement the robotic arm or magnet to pick up food items.
   * **Integration**: Integrate the picking mechanism with the robot’s navigation system.

#### Final Considerations:

* **Testing and Validation**: Conduct thorough testing to ensure the robot can accurately pick up and deliver food items.
* **Iterative Improvements**: Based on testing results, iteratively improve the robot’s design, navigation, and deep learning models.

#### Summary:

* Ensure the robot can handle different food items with a reliable picking mechanism.
* Simplify navigation with QR codes and straight-line paths where possible.
* Develop and train deep learning models for accurate identification and localization of food items and animals.
* Focus on a clear operational flow from food item identification to delivery.
