# 🌊 Wave Data Analysis – Copernicus Marine Virtual Buoy Explorer

This repository provides a student-friendly interactive notebook to **download, visualize, and analyze global wave data** from the [Copernicus Marine Service (CMEMS)](https://marine.copernicus.eu/).

The tool is built for **educational and research purposes**, enabling students and researchers to explore long-term wave conditions, identify extreme events, and generate return period statistics directly from reanalysis data.

> 🧪 Designed to run in **Google Colaboratory**, with automatic Google Drive integration and output folders for data and plots.

🎬 [Watch the full tutorial on YouTube](https://youtu.be/iTavyBcSzu0)

---

## 🚀 Features

- 📦 Downloads **global wave reanalysis data** (`GLOBAL_REANALYSIS_WAV_001_032`)
- 🧭 Lets you define a **study area and a virtual wave buoy**
- 🗺 Visualizes wave height, period, and direction on maps (with vector arrows and contours)
- 📈 Plots **time series**, **wind roses**, and **heatmaps**
- 🔍 Detects and plots **extreme wave events**
- 📊 Performs **return period analysis** using **Gumbel** and **GEV** distributions with bootstrap confidence intervals
- 🔥 Includes **climate strips** and **monthly anomaly heatmaps**
- 💾 Exports data and graphics to organized folders

---

## 📁 Included Example Files

This repository includes example data and a structured layout to get you started:

```
wave_data_downloader/
├── notebook.ipynb                ← Main analysis notebook
```

---

## 🧪 How to Use It (Google Colab)

This notebook is meant to be run in **Google Colaboratory** using files saved in your **Google Drive**.

### 📥 Step-by-step:

1. **Download this repository** as a ZIP:
   - Click the green **`Code`** button at the top of this page
   - Select **`Download ZIP`** and extract locally

2. **Upload the folder to your Google Drive**:
   - Suggested path: `My Drive/CoastalHydrodynamics/wave_data_downloader/`

3. **Open the notebook in Google Colab**:
   - Right-click the `.ipynb` file in Drive → **"Open with" → Google Colaboratory**

4. **Follow the steps in the notebook**:
   - Mount Google Drive
   - Set working directory and area of interest
   - Download data (once only)
   - Run visualization and analysis

> ✅ All plots and outputs are automatically saved in the `output_images/` and `output_data/` folders.

---

## 🌐 Required Registration

To download data, you must:

- 🔓 Create a free account at [marine.copernicus.eu](https://marine.copernicus.eu/)
- 🔐 Log in via code using:
  ```python
  copernicusmarine.login()
  ```

---

## 📦 Dependencies

The notebook uses the following Python libraries (pre-installed in Google Colab):

- `copernicusmarine`, `xarray`, `numpy`, `pandas`
- `matplotlib`, `cartopy`, `seaborn`, `scipy`
- `plotly`, `ipywidgets`, `windrose`

---

## 📚 References

- 📄 **Wave Data Source**: `GLOBAL_REANALYSIS_WAV_001_032`  
  [🔗 DOI: 10.48670/moi-00022](https://doi.org/10.48670/moi-00022)  
  Law-Chune et al. (2021), *Ocean Dynamics*, [https://doi.org/10.1007/s10236-020-01433-w](https://doi.org/10.1007/s10236-020-01433-w)

- 🧭 **Copernicus Marine Service**:  
  https://marine.copernicus.eu/

---

## 📝 Acknowledgments

This script was developed by **Alessio Rovere** at **Ca' Foscari University of Venice**, with the support of **ChatGPT by OpenAI** for code structuring, optimization, and documentation refinement.

This work is part of the **WARMCOASTS** project, funded by the **European Research Council (ERC)** under the European Union’s Horizon 2020 research and innovation programme (grant agreement n. **802414**).

⚠️ **Disclaimer:**  
The code is provided *as is*, without warranties of any kind. Users are responsible for verifying outputs and adapting the scripts to their needs. Neither the authors nor the European Union can be held liable for outcomes resulting from the use of this tool.

---

## 📘 Citation

If you use this notebook in teaching, publications, or derivative works, please cite the original dataset and link to this repository.
---

## 📬 Contact

For feedback or suggestions, open an issue on GitHub or reach out to the project maintainer.
