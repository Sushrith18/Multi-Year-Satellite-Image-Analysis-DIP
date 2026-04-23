# 🌍 Multi-Year Satellite Image Analysis using Digital Image Processing (DIP)

---

## 📌 Overview
This project focuses on applying **Digital Image Processing (DIP)** techniques to analyze multi-year satellite imagery (2021–2025) obtained from **Google Earth Engine (GEE)**.

The goal is to extract meaningful insights related to:
- 🌱 Vegetation using NDVI  
- 💧 Water bodies using NDWI  
- 🧹 Noise removal using filtering  
- 🧩 Image segmentation  
- 📦 Image compression  
- 🔍 Feature extraction and enhancement  

---

## 🎯 Objectives
- Process Sentinel-2 satellite images  
- Compute NDVI & NDWI  
- Apply filtering techniques and evaluate using PSNR & SSIM  
- Perform segmentation using Otsu & K-Means  
- Analyze compression impact  
- Extract features using edge detection, CLAHE, and morphology  

---

## 🛰️ Dataset
- **Source:** Google Earth Engine  
- **Satellite:** Sentinel-2  
- **Years Covered:** 2021 – 2025  

### 📡 Bands Used

B3 → Green
B4 → Red
B8 → NIR


---

## 🧠 Techniques Used

### 1️⃣ Spectral Indices
- NDVI (Vegetation Analysis)  
- NDWI (Water Body Detection)  

### 2️⃣ Filtering
- Gaussian Filter  
- Median Filter  
- Bilateral Filter  
- Wiener Filter  

### 3️⃣ Segmentation
- Otsu Thresholding  
- K-Means Clustering  

### 4️⃣ Compression
- JPEG (Low & High Quality)  
- PNG (Lossless)  

### 5️⃣ Feature Extraction
- Canny Edge Detection  
- CLAHE (Contrast Enhancement)  
- Morphological Operations  

---

## 📊 Results

- Wiener filter achieved the highest **PSNR & SSIM**  
- Otsu segmentation performed better than K-Means  
- NDVI effectively identified vegetation  
- NDWI successfully detected water bodies  
- Compression impacted segmentation accuracy  

---

## 📈 Water Body Analysis (2021–2025)

| Year | Water Area (km²) | NDWI Mean | Change vs 2021 (%) |
|------|------------------|-----------|--------------------|
| 2021 | 6.47 | -0.071 | Baseline |
| 2022 | 6.46 | -0.128 | -0.30 |
| 2023 | 4.57 | -0.118 | -29.45 |
| 2024 | 2.53 | -0.122 | -60.97 |
| 2025 | 5.48 | -0.089 | -15.36 |

---

## 📂 Project Structure


Multi-Year-Satellite-Image-Analysis-DIP/
│
├── gee_exports/ # Input satellite images (.tif)
├── report_assets/ # Output images (NDVI, NDWI, etc.)
├── notebook.ipynb # Google Colab / Jupyter Notebook
├── report.pdf # Final project report
└── README.md


## ⚙️ Installation

pip install rasterio numpy matplotlib opencv-python scikit-image
▶️ Usage
1. Download Sentinel-2 images using Google Earth Engine  
2. Place all .tif files inside the 'gee_exports/' folder  
3. Run the notebook step-by-step  
4. Output images will be saved in 'report_assets/'  
🔍 Key Observations
Vegetation areas are easier to segment due to high NDVI contrast
Water bodies are clearly identified using NDWI
Urban areas are difficult due to mixed pixel values
Compression reduces quality and affects segmentation accuracy
🚀 Future Improvements
Deep Learning-based segmentation (CNNs, U-Net)
Multi-band and hyperspectral analysis
Time-series prediction of land-use changes
Integration with GIS platforms
📚 References
Google Earth Engine
Sentinel-2 Dataset
Digital Image Processing – Gonzalez & Woods
Rasterio Documentation

👤 Author:
N. Sushrith Sai


