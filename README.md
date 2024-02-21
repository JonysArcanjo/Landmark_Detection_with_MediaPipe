
[![Medium](https://img.shields.io/badge/Medium-%23000000.svg?style=for-the-badge&logo=Medium&logoColor=white)](https://medium.com/@jonysarcanjo) [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&labelColor=blue)](https://www.linkedin.com/in/jonysarcanjo/)[![MediaPipe](https://img.shields.io/badge/MediaPipe-%23000000.svg?style=for-the-badge&logo=mediapipe&logoColor=white)](YOUR_MEDIAPIPE_LINK_HERE) [![OpenCV](https://img.shields.io/badge/OpenCV-green?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/) [![Python](https://img.shields.io/badge/Python-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/) [![Computer Vision](https://img.shields.io/badge/Computer%20Vision-%23000000?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAWElEQVQ4T2NkIAoYf/58+Q8YRiQRMyAaMgPjEGMEAzMDI8RAbGgYGBgEGMEIiAyNAAYxAyMDI8RAbGgYJoNjYGBgYBBlZmZmoIJRYPj/8+fPf2HkYGBgAADJAxMFtDq5TAAAAABJRU5ErkJggg==&logoColor=white)](YOUR_LINK_HERE)




[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
# Landmark Detection with MediaPipe

![CAPA Medium (2)](https://github.com/JonysArcanjo/Landmark_Detection_with_MediaPipe/assets/48812740/d8df1ea1-e783-484a-964a-b3f077e20702">)


## Project Objective

🚀 In this project, we explore the power of MediaPipe, an open-source platform developed by Google, to simplify the development of multimedia applications. Specifically, we utilize the BlazePose model GHUM 3D to detect and analyze 33 body landmarks, providing a comprehensive three-dimensional representation for accurate pose estimation. Enhance your applications with intuitive visualization and detailed performance analysis using this robust framework. 🌐✨


# Evolution of Face Detection Algorithms

Over time, various face detection algorithms have been developed, each with its merits and specific applications. Beginners in the field may feel overwhelmed by the diversity of available tutorials – some focusing on Haar Cascades, others on the dlib library, and more recently, the rise of MediaPipe, which has gained prominence to the point of overshadowing traditional alternatives like the Single Shot Multibox Detector (SSD).

To illustrate this evolution and aid in understanding this field, the figure below (taken from the article [What is Face Detection](https://learnopencv.com/what-is-face-detection-the-ultimate-guide/)) provides an overview of algorithms over time. **But how to navigate through this variety without getting lost? How to make the best decision for your application?**

![Images](https://github.com/JonysArcanjo/Landmark_Detection_with_MediaPipe/assets/48812740/80ea39c8-6022-4aba-a993-2727b28b57c8)

## Choosing the Ideal Model

The perfect model for face detection should align with the unique requirements of your project. The author of the mentioned article suggests that the decision should be based on three fundamental criteria:

**Superior Detection Accuracy:** If the priority is to capture each face with the highest accuracy possible, the DSFD or RetinaFace-resnet50 algorithms emerge as the best choices. However, it's essential to be aware that the high complexity of such models results in reduced inference speed, which can be a hindrance for real-time applications.

**Maximum Detection Speed:** If the emphasis is on the speed of inference, even if it means sacrificing some detections in complex scenarios, the MediaPipe face detection solution is the ideal alternative.

**Best cost-benefit between speed and accuracy:** For those seeking a middle ground, the YuNet and RetinaFace-Mobilenetv1 models present themselves as balanced candidates. They offer fast inference speed suitable for real-time applications without excessively sacrificing accuracy.

Selecting the correct algorithm is a decisive step that can determine the success of your application. We will specifically work with:

- OpenCV's DNN module
- MediaPipe Solutions

## MediaPipe

**MediaPipe** is an open-source platform for creating situational awareness solutions. Provided by Google, it offers a framework for building applications and solutions that require processing multimedia data streams, including but not limited to video, audio, and sensor data. **MediaPipe** was created with the mission of accelerating the development cycle of multimedia applications on various platforms.

For the *Pose Estimation* task, we will use **MediaPipe** to:

1. **Detect and draw *pose landmarks***: MediaPipe will allow us to identify key points of the body, or *landmarks*, and draw them on our images and videos for a more intuitive visualization.
2. **Draw *landmark connections***: In addition to detecting individual *landmarks*, MediaPipe also allows drawing connections between them, facilitating the understanding of overall posture.
3. **Get the pixel coordinates of the *landmark***: With MediaPipe, we will be able to extract the coordinates of the pixels corresponding to each *landmark*, enabling more detailed analyses.

### 4.3.1 - Pose Landmark Model - BlazePose GHUM 3D

The *landmark* model for pose estimation that we will use is **BlazePose GHUM 3D**, also offered by Google through **MediaPipe**. This model provides a complete 3D representation of the human body, including 33 *landmarks* that cover the entire body.

![BlazePose GHUM 3D](https://sigmoidal.ai/wp-content/uploads/2023/07/68747470733a2f2f6d65646961706970652e6465762f696d616765732f6d6f62696c652f706f73655f747261636b696e675f66756c6c5f626f64795f6c616e646d61726b732e706e67.png)

The *BlazePose GHUM 3D* model has been trained on a large dataset of human poses and movements, allowing it to accurately predict body *landmarks* even in different poses and orientations. This makes it a powerful tool for our sports performance analyses. See the complete list of *landmarks* for reference.


**Features**:
- Detect faces in images and videos.
- Visual display of facial landmarks on the original image.

Perfect for applications in facial recognition, emotion detection, and other advanced computer vision tasks.

## Project Structure

```
.
├── Readme.md
├── landmarkImagem.py
├── landmarkVideo.py

```
## Used Libraries

This project requires the following libraries:

- OpenCV
- Mediapipe
- Numpy

## Conclusion

Through the two scripts presented, it becomes clear how accessible and effective the construction of a facial landmark detection system is. With the right tools and libraries, it's possible to demystify its complexity and implement it in a simplified manner. 

This ability to identify and mark specific points on the face opens doors to a range of applications, from facial recognition to deeper analyses of expressions and emotions. By mastering these scripts, we can venture into new horizons in computer vision and further explore the potentialities of facial detection.

## Contact
[![LinkedIn](https://img.icons8.com/color/32/000000/linkedin.png)](https://www.linkedin.com/in/jonysarcanjo/)

[![Medium](https://img.icons8.com/color/32/000000/medium-logo.png)](https://medium.com/@jonysarcanjo)

e-mail: contato.jonysarcanjo@gmail.com


## License

This project is licensed under the MIT License.


