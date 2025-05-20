# 🏙️ Devanahalli Airport Urbanization Change Analysis

This project analyzes urban expansion around **Kempegowda International Airport (Devanahalli, Bangalore Rural)** using multi-temporal satellite imagery (Landsat-8 and Sentinel-2) and land cover classification from ESA WorldCover data. It visualizes how urban development has progressed in and around the airport area over the years, highlighting the impact of infrastructure-driven growth.

---

## 📌 One-line Summary

**Analyzes urbanization change around Devanahalli Airport using satellite imagery and land cover classification.**

---

## 🛰️ Data Sources
- **Sentinel-2 RGB (2018–2023)**: Higher-resolution imagery for recent development.

---

---

## 🧠 Methods Used

- Satellite image preprocessing and visualization
- (Optional) NDVI computation for vegetation cover analysis
- Deep learning-based semantic segmentation (e.g., U-Net)
- Classification into urban vs. non-urban areas
- Year-over-year change detection and trend analysis

---

## 📊 Output

- Urban area segmentation masks for each year
- Change detection maps showing urban growth patterns
- Quantitative statistics (e.g., urbanized % area per year)
- Comparative plots and visualizations

---

## 📦 Main Libraries Used

- `numpy` – For array and numerical computations  
- `matplotlib` – For plotting and visualization  
- `rasterio` – To read and write raster (GeoTIFF) data  
- `opencv-python` – For image processing operations  
- `tensorflow` or `torch` – For deep learning-based segmentation (U-Net or other models)  
- `scikit-learn` – For preprocessing, metrics, or clustering if used  

---

## 🚀 How to Run

1. Place the satellite imagery files in their respective folders inside `GEE_Exports/`

2. Open the notebook:  
`Bangalore_Urbanization_Change.ipynb`

3. Run all the cells in sequence.

4. Visualize and interpret:
- Urban area masks over time
- Change detection maps
- Statistics and trends in urban expansion

---

## ⚙️ Working of the Code

1. **Importing Dependencies**  
All necessary Python libraries are imported (e.g., `rasterio`, `matplotlib`, `numpy`, etc.) for geospatial and deep learning tasks.

2. **Loading Satellite Data**  
GeoTIFF images from Sentinel-2 are read using `rasterio`. Images are displayed using `matplotlib`.

3. **Preprocessing**  
- Bands are normalized and resized if necessary.
- Data is cleaned and formatted for modeling.

4. **Urban Classification**  
Pixels are classified as **urban** or **non-urban** using either:
- ESA's label data directly, or
- Predicted masks from segmentation models

5 **Change Detection**  
Urban masks from different years are compared to:
- Identify newly urbanized regions
- Quantify area change (e.g., total urban area in hectares or km²)

6. **Visualization & Statistics**  
- Time series plots
- Side-by-side RGB vs. classified maps
- Statistical tables of urban area change over years

---

## 📌 Use Cases

- Assessing infrastructure-led urbanization
- Supporting urban planning near major airports
- Monitoring green cover loss due to expansion
- Identifying zones of rapid development for policy response

---



