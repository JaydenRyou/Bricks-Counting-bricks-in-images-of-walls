## Bricks: Counting bricks in images of walls

### Introduction
Welcome to our final project for Math 490 (Computational Math). Our project focuses on measuring the height of buildings on the University of Illinois Urbana Champaign campus, which are primarily constructed with bricks or have brick facades. Traditionally, the height of these buildings can be determined by counting the layers of bricks. This approach provides a simple yet effective way of determining building height.

For this project, we will manually implement code using popular Python libraries such as NumPy and Scipy, without relying on the OpenCV module. However, to ensure our code is implemented correctly, we will use OpenCV as a ground truth. Through this project, we aim to showcase the power of computational math and how it can be applied to solve real-world problems.

### Brief Overview
Our project aims to perform edge detection using the Canny edge detection technique. The process involves the following steps:

1. Noise reduction: We will first remove noise from the image to obtain a cleaner edge map.
2. Gradient calculation: Next, we will calculate the gradient of the image to identify regions with the strongest edge.
3. Non-maximum suppression: We will then perform non-maximum suppression to thin out the edges and ensure that only the strongest edges are preserved.
4. Local maximum counting: After obtaining an equation through interpolation and applying a Gaussian filter, we will count the number of local maxima in the vertical line of the image to determine the number of brick layers.
5. Brick counting with OpenCV: We will count the number of bricks or layers in the image using OpenCV to determine the height of the building.
6. Accuracy comparison: Finally, we will compare the results of our model with the ground truth obtained from OpenCV and assess its accuracy.

By the end of the project, we aim to provide an effective and accurate method for edge detection that can be applied to a range of real-world applications.

**Original Image**             |  **Non-maximum suppression**
:-------------------------:|:-------------------------:
<img src="https://raw.githubusercontent.com/JaydenRyou/Bricks-Counting-bricks-in-images-of-walls/main/Bricks%20Image/Bricks.jpg"  width="30%" height="10%"> | <img src="https://github.com/JaydenRyou/Bricks-Counting-bricks-in-images-of-walls/blob/main/Bricks%20Image/NMS_bricks.png"  width="30%" height="10%">
**Vertical line data**    | **Gaussian filtered data**
<img src="https://github.com/JaydenRyou/Bricks-Counting-bricks-in-images-of-walls/blob/main/Bricks%20Image/vertical_line.png"  width="80%" height="80%"> | <img src="https://github.com/JaydenRyou/Bricks-Counting-bricks-in-images-of-walls/blob/main/Bricks%20Image/filtered%20data.png"  width="50%" height="50%">
