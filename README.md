# Human Activity Recognition with CNN (Multimodal)

Project for recognition physical activity using multimodal data (Kinect, IMU, EMG).

## Abstract.

This work aims to develop a methodology for recognizing 5 physical activities from data collected by a multimodal sensor network consisting of Kinect, IMU, and EMG. To achieve this was proposed a method based on primitive motion detection, inspired by speech recognition models. Primitive movements are the simplest sub-movements into which the activity is divided. Encoding these primitive movements into a single discriminant sequence allows for the recognition of the physical activity.

This work focuses primarily on the recognition of primitive motions using Convolutional Neural Networks (CNNs). These models can work with time series data, demonstrating the ability to extract repetitive patterns and classify repetitive motions within a short time window. Two types of CNN architectures for primitive motion classification are analyzed: the MultiHead model (CNN1D), specifically designed for working with one-dimensional time series data (input vector), and the LarModel architecture (CNN2D), which requires transforming the data into a 3D matrix structure similar to an image channel.

The results show that both CNN methodologies achieve comparable performance to state-of-the-art methodologies, with the MultiHead model achieving better performance (85%) than the LarModel (80.63%) for all three sensor modalities. In physical activity recognition using the HMM model, the LarModel methodology performs better with Kinect (97.00%) and EMG (76.11%) sensors, while the MultiHead model performs better with IMU (89.92%). Multimodal sensor fusion shows better performance than individual sensors, demonstrating that combining each sensor provides important information for improving classification, with the Kinect-IMU combination achieving the best average performance.

## 🚧 Project Status
Initial version with notebook:
* CNN_HAR_Clasification.ipynb - complete project code
* Time_Series_codes.ipynb - test code for working with time series

## 📁 Structure
- notebooks/: experiments in Colab
- data/:
