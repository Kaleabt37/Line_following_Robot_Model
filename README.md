# Line_following_Robot_Model_Using(CNN)
This repository contains a project that demonstrates a line following robot model built using computer vision and deep learning techniques. The project leverages an image datasets extracted from a 10-second YouTube video and utilizes Convolutional Neural Networks (CNNs) to train the model that classifies motion directions (straight, right, and left).

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Libraries and Dependencies](#libraries-and-dependencies)
- [Credits](#credits)
- [License](#license)

## Project Overview

The project is divided into three main stages:

1. **Frame Extraction**  
   - **Source:** A 10-second YouTube video.
   - **Process:** Frames are extracted using the `Frame_Extraction.ipynb` notebook.
   - **Output:** Two types of frames are generated:
     - **Extracted Frames:** The original frames from the video.
     - **Inverted Frames:** Frames with inverted colors are created to balance the dataset (since most frames are straight/right turning, while left-turning frames occur less frequently).

2. **Frame Renaming (Labeling)**  
   - **Process:** After manual classification, frames are moved into three labeled folders: `straight`, `right`, and `left`.
   - **Automation:** The `rename.py` script (inside the `2_Frame_Renaming` folder) automatically renames each image to the format `foldername_0000.jpg`, where the number increments for each frame.

3. **Model Training**  
   - **Process:** The labeled dataset is used to train a CNN model in the `Line_following_model.ipynb` notebook located in the `3_Model_Training` folder.
   - **Output:** The trained model is saved as `Line_following_Robot_cnn.h5`.

## **Installation**  
### **1. Clone the Repository**  
```bash
git clone https://github.com/your-username/Line_Following_Robot.git
cd Line_Following_Robot
```
### **2. Install Dependencies** 
Make sure you have Python 3.8+ installed. Run the following command to install necessary libraries:
```bash
pip install -r requirements.txt
```
## **Usage** 
### **1. Extract Frames**
Run the Jupyter notebook to extract frames from the video:
```bash
cd Frame_Extraction
jupyter notebook Frame_Extraction.ipynb
```
### **2. Label and Rename Data**  
```bash
cd Frame_Renaming
python rename_images.py
```
### **3. Train the Model**  
```bash
cd Model_Training
jupyter notebook Line_following_model.ipynb
```
## **Dependencies**
This project requires the following Python libraries:

- OpenCV (`cv2`)
- TensorFlow
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

All dependencies are listed in requirements.txt
## **Authors**
This project was developed by Kaleab Tesfaye and Abdulbasit Hamid
## **License**
This project is licensed under the MIT License – see the LICENSE file for details







