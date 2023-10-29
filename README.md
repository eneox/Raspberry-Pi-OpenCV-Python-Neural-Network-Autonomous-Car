# OpenCV-Python-Neural-Network-Autonomous-Car

## Project Description

The goal of this exciting project is to create a fully autonomous car leveraging the power of neural networks, with a focus on integrating the OpenCV and TensorFlow libraries using the Python programming language. Let's delve into the key components of the project:

- **Raspberry Pi:** Known for its small size, low power consumption, and extensive hardware support, the Raspberry Pi serves as the brain of the project.

- **L298N Motor Driver:** A motor driver card used to control DC motors. It is responsible for directing the movement of the car in the project.

- **DC Motor:** DC motors are used to provide motion for the car. They are controlled through the L298N Motor Driver.

- **Samsung 18650 Li-ion Battery:** To power the L298N Motor Driver and other components, the project utilizes Samsung 18650 Li-ion batteries. These batteries provide a reliable and rechargeable power source for the autonomous car.

- **Webcam Camera:** The project incorporates a webcam camera to capture real-time visual data. This webcam, interfaced through the OpenCV library, provides the car with a continuous stream of images for analysis and decision-making.

- **Lane Detection Using Hough Line Transform and Pixel Analysis:** To enable the car to follow a white lane, the project combines the power of Hough Line Transform with pixel analysis. Pixel analysis involves thresholding the image to identify white pixels, and Hough Line Transform is then applied to detect line segments. By analyzing pixel clusters associated with the detected lines, the algorithm accurately determines the position and orientation of the lane markings, allowing the car to navigate autonomously.

- **Motor Control Through Neural Networks:** The autonomous car's movements are controlled by a neural network implemented through TensorFlow. The neural network processes the information gathered from the webcam and determines the appropriate actions. For instance, if the car detects a deviation from the center of the lane, the neural network instructs the motors through the L298N Motor Driver to adjust the direction, maintaining a smooth and centered trajectory. The neural network is trained to make decisions such as moving forward, backward, turning left, or turning right based on the analysis of the visual data.

  - **Forward Motion:** Neural network signals the L298N Motor Driver to power the DC motors in a forward direction, propelling the car along the designated path.

  - **Backward Motion:** If necessary, the neural network triggers reverse movement by instructing the L298N Motor Driver to change the polarity of the DC motors, enabling the car to navigate in reverse.

  - **Steering Control:** To steer the car, the neural network adjusts the relative speeds of the DC motors. Differentially varying the speeds of the left and right motors allows the car to make smooth turns, ensuring it stays centered within the lane.

## Integration of OpenCV and TensorFlow

In order to enhance the autonomous capabilities of the car, the project incorporates the following key technologies:

- **OpenCV:** The OpenCV library is employed for computer vision tasks, enabling the car to process and interpret visual data. This is essential for tasks such as object detection, lane tracking, and overall scene understanding.

- **TensorFlow:** Leveraging the power of TensorFlow, the project integrates neural networks to facilitate advanced decision-making processes. This includes training models for object recognition, navigation, and other critical functions vital for autonomous driving.

By combining the strengths of OpenCV and TensorFlow, and integrating a webcam camera along with pixel analysis and Hough Line Transform for lane detection, the autonomous car project achieves a robust and intelligent system capable of making real-time decisions based on its environment.

![image](https://github.com/eneox/Raspberry-Pi-OpenCV-Python-Neural-Network-Autonomous-Car/assets/96574231/dab9a508-6386-4a71-bde9-cae24b9697a6)
