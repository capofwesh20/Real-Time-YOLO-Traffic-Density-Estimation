# Real-Time-YOLO-Traffic-Density-Estimation

![Real-time Analysis](https://github.com/capofwesh20/Real-Time-YOLO-Traffic-Density-Estimation/assets/35642413/174b86bc-2ba7-42df-b138-2394014ed2b2)

![image](https://github.com/capofwesh20/Real-Time-YOLO-Traffic-Density-Estimation/assets/35642413/ad717cd2-7c2e-40b4-9f78-246b5623845b)

## Traffic Density Estimation Project Overview**

This project capitalizes on the real-time detection strengths of YOLO to concentrate on estimating traffic density, a crucial aspect of urban and traffic administration. Its main objective is to enumerate vehicles in designated areas across each video frame, facilitating an evaluation of traffic congestion. The gathered information is instrumental in pinpointing high-traffic intervals and areas of congestion, thereby contributing to urban development planning. The endeavor is geared towards creating an extensive toolkit that offers in-depth analysis of traffic movement and trends, ultimately improving strategies for traffic control and urban planning.

## Project Objectives

1. **Selection and Preliminary Evaluation of YOLOv8**: Initiating the project with the selection of a pre-trained YOLOv8 model, followed by an initial evaluation of its performance on the COCO dataset specifically for vehicle detection tasks.

2. **Creation of a Specialized Vehicle Dataset**: Developing a curated and annotated dataset focused on vehicles. This dataset aims to improve the model's capability to recognize various types of vehicles accurately.

3. **Fine-Tuning the Model for Superior Vehicle Detection**: Applying transfer learning to adjust the YOLOv8 model for enhanced detection of vehicles, particularly from aerial views, to achieve better precision and recall in the detection process.

4. **In-Depth Evaluation of Model Performance**: Conducting a thorough assessment of the model through the analysis of learning curves, a confusion matrix, and other performance metrics to ensure the model's accuracy and its ability to generalize across different scenarios.

5. **Testing Model Inference and Generalization**: Evaluating the model's generalization capabilities on a set of validation images, an unseen test image, and a test video to showcase its practical utility and effectiveness in real-world applications.

6. **Real-Time Traffic Density Analysis**: Implementing an algorithm capable of estimating traffic density in real time by counting vehicles and assessing traffic intensity through analysis of test video data.

7. **Preparation for Cross-Platform Deployment**: Preparing the fine-tuned model for deployment across various platforms by exporting it in ONNX format, ensuring compatibility and ease of integration into different software environments.

# 📚 Dataset Description
🌐 Overview
The Top-View Vehicle Detection Image Dataset for YOLOv8 is essential for tasks like traffic monitoring and urban planning. It provides a unique perspective on vehicle behavior and traffic patterns from aerial views, facilitating the creation of AI models that can understand and analyze traffic flow comprehensively.

# 🔍 Specifications
**🚗 Class: 'Vehicle' including cars, trucks, and buses.**
**🖼️ Total Images: 626
**📏 Image Dimensions: 640x640 pixels**
**📂 Format: YOLOv8 annotation format**
#🔄 Pre-processing
Each image is carefully pre-processed and standardized to ensure consistency and high-quality training data for our model.

#🔢 Dataset Split
The dataset is meticulously split into:

**Training Set: 536 images for model training with diverse scenarios.**
**Validation Set: 90 images for unbiased model performance evaluation.**
#🎭 Augmentation on Training Set
Augmentations, including horizontal flips, are applied to enhance the training set's robustness, ensuring the model learns to generalize well across varied traffic conditions.


# Exploring the Model Development Pipeline
Get hands-on with the model development process and see the results of traffic density estimation:

**Download the Dataset:** Access the dataset from the link in the notebook. Download and extract it to a known directory on your machine.
**Open the Notebook:** Launch Jupyter Notebook or JupyterLab and open real-time_traffic_density_estimation_yolov8.ipynb to explore the model development pipeline.
**Install Dependencies:** Ensure all necessary Python libraries are installed for flawless execution.
**Update Paths:** Update the paths in the notebook for the dataset, sample image, and sample video to their respective locations on your local system.
**Run the Notebook:** Execute all cells in the notebook to step through the data preprocessing, model training, and evaluation phases.


### 3️⃣ Watching the Real-Time Performance

Witness the real-time traffic analysis capability of our YOLOv8 model:

#### Install Ultralytics YOLO
Ensure you have the ultralytics package installed by running:
```bash
pip install ultralytics
```

#### Run the Analysis Script
With the Ultralytics package installed, you're ready to execute the script that powers the real-time traffic density estimation. Run the following command from the root directory of the project:
```bash
python Real_time_analysis.py
```

#### Real-Time Analysis
Once the script is running, a video window will open, displaying the live traffic analysis. This window will show the YOLOv8 model in action, detecting vehicles and estimating traffic density in real time.

To close the video window and exit the analysis, simply press 'q' while the video window is active.

