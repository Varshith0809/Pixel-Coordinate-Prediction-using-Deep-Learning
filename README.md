# Pixel Coordinate Prediction using Deep Learning

## 📌 Problem Statement
Given a 50×50 grayscale image where exactly one pixel has a value of 255
and all others are 0, predict the (x, y) coordinates of the bright pixel
using Deep Learning techniques.

## 🧠 Approach
- The problem is framed as a **supervised regression task**
- Input: 50×50 grayscale image
- Output: Normalized (x, y) coordinates of the bright pixel
- A **Convolutional Neural Network (CNN)** is used to learn spatial features

## 📊 Dataset Generation
- Synthetic dataset is generated since no real dataset exists
- Each image contains one randomly positioned bright pixel
- Pixel values are normalized to [0, 1]
- Coordinates are normalized by dividing by 49

## 🏗 Model Architecture
- Convolutional layers for spatial feature extraction
- MaxPooling layers for dimensionality reduction
- Fully connected layers for coordinate regression
- Output layer has 2 neurons representing (x, y)

## ⚙️ Dependencies
```bash
pip install numpy matplotlib tensorflow
