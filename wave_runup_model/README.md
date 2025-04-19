# 🌊 Wave Runup Calculator – IPCC-Aware Coastal Flooding Tool

This repository provides an interactive Python notebook designed to **calculate wave runup** using field data (wave and tide measurements) and **project future runup scenarios under sea-level rise**, based on **IPCC AR6 projections**.

The tool is intended for **educational use** (e.g., in Earth Science or Environmental Engineering courses), but can also serve as a lightweight exploratory model for research and coastal planning.

> 🧪 Designed to be used in **Google Colaboratory**, with example datasets included.

---

## 🚀 Features

- 📈 Loads and visualizes **wave buoy** and **tide gauge** data
- 🌊 Calculates **wave runup** using 8 published empirical models (via [`py-wave-runup`](https://py-wave-runup.readthedocs.io))
- 🔮 Integrates **IPCC AR6 sea-level rise projections** (median and full quantile range)
- 📊 Produces plots of:
  - Wave + tide time series
  - Runup histograms and KDEs (present-day vs. future)
  - Time series of maximum runup with and without sea-level rise
- 💾 Exports runup data for further use or visualization

---

## 📁 Included Example Files

This repo includes a set of example files to help you get started:

- `Tide_Gauge.csv` — sample water level data (timestamp + tide height)
- `Wave_buoy.csv` — sample wave data (Hs, Tmean, etc.)
- `ipcc_ar6_sea_level_projection_psmsl_id_59.xlsx` — IPCC AR6 projections for a tide station

> ✅ These files are automatically loaded in the example notebook, so you can start experimenting right away.

---

## 🧪 How to Use It (Google Colab)

This notebook is designed to run in **Google Colaboratory**, using files stored in your own **Google Drive**.

### 📥 Step-by-step instructions:

1. **Download this repository** as a ZIP file:
   - Click the green **`Code`** button at the top of this page
   - Choose **`Download ZIP`**
   - Unzip the folder on your computer

2. **Upload the folder to your Google Drive**:
   - Place it in a location you can easily find (e.g., `My Drive/Runup/`)

3. **Open the notebook** in Google Colab:
   - Right-click on the notebook file (`.ipynb`) in Google Drive
   - Select **“Open with” → “Google Colaboratory”**

4. **Follow the instructions in the notebook**:
   - Mount your Drive
   - Set the working directory
   - Load data and run calculations
   - Visualize and export results

> ✅ All required data files are already included in the repo. You just need to upload the folder and start exploring.

---

## 📦 Dependencies

The notebook uses the following main packages:

- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `ipywidgets` (for dropdowns)
- [`py-wave-runup`](https://py-wave-runup.readthedocs.io) (included locally in the repo)

All required packages are pre-installed in Google Colab. No local setup needed.

---

## 📚 Acknowledgements

- This tool uses the open-source [`py-wave-runup`](https://py-wave-runup.readthedocs.io) package by Chris Leaman and contributors.
- Sea-level projections are sourced from the **NASA IPCC AR6 Sea-Level Projection Tool**:  
  https://sealevel.nasa.gov/ipcc-ar6-sea-level-projection-tool

---

## 📝 Acknowledgments

This script was developed by **Alessio Rovere** at **Ca' Foscari University of Venice**, with the support of **ChatGPT by OpenAI** for code structuring, optimization, and documentation refinement.

This work is part of the **WARMCOASTS** project, funded by the **European Research Council (ERC)** under the European Union’s Horizon 2020 research and innovation programme (grant agreement n. **802414**).

⚠️ **Disclaimer:**  
The code is provided *as is*, without any warranties or guarantees of correctness. Users are responsible for verifying results and adapting the scripts to their specific needs. Neither the authors nor the European Union can be held responsible for any use that may be made of the information or code contained herein.

---

## 📘 Citation

If you use or adapt this notebook for teaching or research, please credit the original authors of the runup models and acknowledge this repository.

---

## 📬 Contact

For questions, suggestions, or feedback, feel free to open an issue or reach out to the repo maintainer.