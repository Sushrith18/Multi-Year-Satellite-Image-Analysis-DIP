# 🌍 Multi-Year Satellite Image Analysis using DIP

📌 Overview

This project focuses on applying Digital Image Processing (DIP) techniques to analyze multi-year satellite imagery (2021–2025) obtained from Google Earth Engine (GEE).

The objective is to extract meaningful insights related to:

Vegetation analysis using NDVI
Water body detection using NDWI
Image quality improvement using filtering
Land-use segmentation
Compression and feature extraction

🎯 Objectives
Process Sentinel-2 satellite images
Compute NDVI & NDWI
Apply filtering techniques and evaluate using PSNR & SSIM
Perform segmentation using Otsu & K-Means
Analyze compression impact
Extract features using edge detection and enhancement
🛰️ Dataset
Source: Google Earth Engine
Satellite: Sentinel-2
Years Covered: 2021 – 2025
Bands Used:
B3 (Green)
B4 (Red)
B8 (NIR)

🧠 Techniques Used
1. Spectral Indices
NDVI (Vegetation Analysis)
NDWI (Water Body Detection)
2. Filtering
Gaussian Filter
Median Filter
Bilateral Filter
Wiener Filter
3. Segmentation
Otsu Thresholding
K-Means Clustering
4. Compression
JPEG (Low & High Quality)
PNG (Lossless)
5. Feature Extraction
Canny Edge Detection
CLAHE
Morphological Operations

📊 Results
Wiener filter achieved highest PSNR & SSIM
Otsu segmentation performed better than K-Means
NDVI effectively identified vegetation
NDWI successfully detected water bodies
Compression affected segmentation accuracy

📈 Water Body Analysis (2021–2025)
Year	Water Area (km²)	NDWI Mean	Change (%)
2021	6.47	-0.071	Baseline
2022	6.46	-0.128	-0.30
2023	4.57	-0.118	-29.45
2024	2.53	-0.122	-60.97
2025	5.48	-0.089	-15.36
   
📂 Project Structure
📦 Multi-Year-Satellite-Image-Analysis-DIP
 ┣ 📂 gee_exports        # Raw satellite images (.tif)
 ┣ 📂 report_assets      # Output images (NDVI, NDWI, etc.)
 ┣ 📜 notebook.ipynb     # Google Colab code
 ┣ 📜 report.pdf         # Final report
 ┗ 📜 README.md
⚙️ Installation
pip install rasterio numpy matplotlib opencv-python scikit-image
▶️ Usage
Download Sentinel-2 images using Google Earth Engine
Place .tif files inside gee_exports/
Run the notebook
Outputs will be saved in report_assets/
📌 Key Learnings
Importance of preprocessing in satellite images
Trade-off between compression and quality
Effectiveness of NDVI & NDWI
Challenges in segmentation of urban areas
🚀 Future Improvements
Deep learning-based segmentation
Multi-band analysis
Time-series forecasting
Integration with GIS tools
📚 References
Google Earth Engine
Sentinel-2 Dataset
Digital Image Processing – Gonzalez & Woods

👤 Author
N. Sushrith Sai

