# Arabic Text Image Segmentation


## 📋 Project Overview
This project focuses on extracting and merging word regions from an image using region-growing segmentation techniques. The process involves identifying regions, computing bounding boxes, measuring distances between regions, and merging close regions based on a threshold.

## 🚀 Features
- **Region Extraction:** Uses a region-growing algorithm to segment words in an image.
- **Bounding Box Calculation:** Computes bounding boxes for each detected region.
- **Distance Measurement:** Measures the distance between bounding boxes to determine closeness.
- **Region Merging:** Merges regions that are close to each other based on a specified threshold.
- **Visualization:** Draws bounding boxes around detected and merged regions for visualization.

## 📊 Libraries Used
- **OpenCV:** Advanced image processing
- **NumPy:** Matrix operations
- **Matplotlib:** Visualization

## 📦 Installation
```bash
# Clone the repository
git clone https://github.com/YacineAitKaci/Arabic-Text-Image-Segmentation.git

# Navigate to the project directory
cd Arabic-Text-Image-Segmentation

# Install required libraries
pip install numpy matplotlib opencv-python
```

## 🖼️ How to Use
1. Run the main segmentation notebook:
```bash
jupyter notebook main.ipynb
```

## 🛠️ Customization
- Adjust "seuil" and "seuil_seed" to modify the sensitivity of region extraction.
- Modify "fusion_seuil" to control how close two regions must be to merge.


## ⚡ Challenges Faced
- **Selecting Seed Points:** The choice of initial seed points greatly affects the segmentation results.
- **Threshold Sensitivity:** The method is highly sensitive to the threshold value, which can lead to under- or over-segmentation.
- **Noise Sensitivity:** Noisy images may cause false region growth, leading to inaccurate segmentation.
- **Computation Time:** Large images with many small regions can result in slow processing.
- **Merging Criteria:** Determining the correct criteria to merge regions without losing important details can be complex.

## 💡 Future Improvements
- **Adaptive Thresholding:** Implement an adaptive thresholding technique to dynamically adjust parameters based on the image characteristics.

- **Machine Learning Integration:** Use machine learning models to improve region classification and merging.

- **Parallel Processing:** Optimize the algorithm using parallel processing to improve performance on large images.
- **Build OCR Model:** Build and train a deep learning model for optical caracter recognition (OCR) using region-growing segmentation technique.

---
