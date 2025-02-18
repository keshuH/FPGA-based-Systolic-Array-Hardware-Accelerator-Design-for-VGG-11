# FPGA-based-Systolic-Array-Hardware-Accelerator-Design-for-VGG-11
This project implements the VGG-11 convolutional neural network architecture on FPGA using a systolic array-based hardware accelerator, aiming to optimize matrix multiplication tasks for high-performance image classification. 

## Introduction
VGG-11 is a deep convolutional neural network architecture widely used for image classification tasks in computer vision applications. It consists of several convolutional layers, activation functions like ReLU, max-pooling layers, and fully connected layers. The goal of this project is to implement the VGG-11 architecture on FPGA using a systolic array-based hardware accelerator, particularly targeting the matrix multiplication tasks within the network, and to simulate the performance of the design.

The systolic array allows for high-speed, parallel processing of CNN computations, making it ideal for accelerating tasks like convolution and matrix multiplication in the VGG-11 architecture. This project explores how systolic arrays can improve computational efficiency and reduce latency in FPGA-based CNN implementations.

## Inspiration Behind the Project
Convolutional neural networks (CNNs) have become the backbone of many modern image classification tasks. However, deploying CNN models on hardware such as FPGAs remains challenging due to the high computational cost of operations like matrix multiplication and convolution. Traditional CPU and GPU accelerations often struggle with high power consumption and latency. Inspired by the need for efficient AI hardware, this project explores FPGA acceleration through systolic arrays to overcome these limitations, specifically targeting the VGG-11 architecture for image classification.

## What This Project Does
This project implements the VGG-11 convolutional neural network on an FPGA platform using a systolic array for hardware acceleration. The project focuses on optimizing matrix multiplication, which is essential for the convolutional layers and fully connected layers in VGG-11. 

The design is fully tested and simulated to verify its functionality and performance. By offloading computationally expensive operations to the FPGA, the goal is to achieve faster processing times and lower power consumption compared to traditional hardware.

### Key Features:
- Implementation of VGG-11 architecture on FPGA
- Use of systolic array for matrix multiplication acceleration
- Simulated performance for verifying efficiency and speed
- Optimizations for image classification tasks

## How We Built It
1. **Designing the VGG-11 Architecture**: We started by mapping the VGG-11 architecture, which includes convolutional layers, activation functions, max-pooling layers, and fully connected layers, onto an FPGA design.
2. **Systolic Array Design**: A systolic array was used to accelerate matrix multiplication, a key component of the convolution and fully connected layers. The systolic array structure ensures parallel computation, reducing the latency for matrix multiplication operations.
3. **FPGA Implementation**: The design was implemented using an FPGA toolchain to target high performance and efficient computation.
4. **Simulation and Testing**: After synthesizing the hardware design, we simulated the performance on the FPGA to analyze the improvements in speed and efficiency.
5. **Optimization**: Various optimizations were made during the design, such as precision reduction and parallelization of operations, to ensure that the design works efficiently within the hardware constraints.

## Challenges We Ran Into
- **Hardware Constraints**: Fitting the entire VGG-11 model, including large matrix multiplication operations, onto the FPGA was a challenge due to limited resources.
- **Optimization for Speed and Power**: Balancing speed and power consumption required careful optimization of the systolic array and parallelization of matrix multiplication operations.
- **Simulation Complexity**: Simulating the entire architecture on FPGA while ensuring accurate performance metrics was a complex task due to the need for precise hardware behavior modeling.

## Accomplishments That We're Proud Of
- Successfully implemented the full VGG-11 model on an FPGA using systolic arrays for acceleration.
- Achieved performance improvements in matrix multiplication, which resulted in a significant speedup for the VGG-11 convolutional layers.
- Demonstrated the practical use of systolic arrays for CNN acceleration, a promising approach for reducing latency and improving power efficiency.

## What We Learned
- Systolic arrays are a powerful tool for accelerating matrix multiplication and can significantly improve the performance of CNN architectures on FPGAs.
- Efficient FPGA implementation requires a balance between computational speed, resource utilization, and power consumption.
- The iterative process of design, simulation, and optimization is crucial for successful FPGA implementations.

## What's Next for the Project
- **Further Optimization**: Future work will focus on optimizing the systolic array design to handle even larger CNN models with more convolutional and fully connected layers.
- **Integration with Other Models**: The design can be extended to support other deep learning models beyond VGG-11, including more complex networks like ResNet and Inception.
- **Real-Time Performance**: We aim to achieve real-time performance for image classification tasks by reducing the overall processing time even further.
- **Scalability**: Research into scaling the design to handle batch processing and real-time video streams is planned for future iterations.



