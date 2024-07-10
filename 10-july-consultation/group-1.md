---
description: Autonomous Parking System
---

# Group 1

1. **Camera Configuration**:
   * **Current Idea**: Using 4 cameras.
   * **Suggestion**: Utilize a **single** camera for navigation to simplify the system. A single camera mounted on the robot should be sufficient for detecting and navigating to parking spots.
2. **Parking Lot Management**:
   * **Requirement**: The system should handle more than one parking lot. Use H detection or CV2 to detect the empty parking lot. Try OpenCV first! Then using YOLO.&#x20;
   * **Steps**:
     1. **Identify Parking Lots**: Implement a method to recognize multiple parking lots.
     2. **Choose a Parking Spot**: Develop an algorithm to select an available parking spot.
     3. **Parking Maneuvers**: Implement both parallel and perpendicular parking algorithms.
        * **Parallel Parking**: Pay special attention to the steering mechanism, as it is more complex.
        * **Perpendicular Parking**: This is typically simpler than parallel parking.

#### Hardware Considerations:

1. **Servos and Wheels**:
   * **Addition**: Consider adding servos for precise control of steering.
   * **Omniwheels**: Use omniwheels to improve maneuverability, allowing the robot to move in any direction without changing its orientation.
2. **Camera Placement**:
   * **Current Idea**: Four cameras.
   * **Suggestion**: Reduce to two cameras if necessary, but ideally, a single camera on the car should suffice. This can reduce complexity and potential issues with data integration from multiple sources.

#### Problem Breakdown:

1. **Subproblem Identification**:
   * Break down the main problem (auto parking) into smaller, manageable subproblems.
   * Examples of subproblems:
     * **Detection**: Detecting the parking lot and available spots.
     * **Navigation**: Navigating to the chosen parking spot.
     * **Parking**: Executing the parking maneuver (parallel or perpendicular).

#### Additional Suggestions:

1. **Algorithm Development**:
   * Use computer vision techniques to process the camera feed and identify parking spots.
   * Develop path planning algorithms to navigate from the current position to the parking spot.
   * Implement control algorithms for smooth and accurate steering and movement during parking.
2. **Testing and Iteration**:
   * Test the system in various conditions to ensure reliability.
   * Iterate on the design based on test results, focusing on improving accuracy and robustness.

#### Final Thoughts:

* Keep the design as simple as possible while ensuring functionality.
* Focus on modular development, allowing each part of the system to be developed and tested independently before integration.

#### Tomorrow Target

* Robotics: Mount Ultrasonic sensor, camera and get them all working.
* Deep Learning: camera model which could find the empty parking lot and find the center, do a prototype.
