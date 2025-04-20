# 🌊 Wave Analysis with Copernicus Marine Data

This notebook allows you to **download, analyze, and visualize global wave data** from the [Copernicus Marine Service](https://marine.copernicus.eu/).  
It is part of the [**CoastalHydrodynamics**](https://github.com/Alerovere/CoastalHydrodynamics) collection for teaching and research on ocean dynamics.

---

## 📦 Features

- ✅ Download **global wave reanalysis data** from the CMEMS `GLOBAL_REANALYSIS_WAV_001_032` product  
- 🧭 Define an **area of interest** and place a **virtual wave buoy**
- 📉 Plot wave height, period, and direction
- 📤 Export data and graphics for reports and analysis
- 📆 Interactively select time intervals for custom analysis
- 📈 Perform **extreme value statistics** and return period calculations (Gumbel + GEV)
- 🔥 Create **heatmaps and strip plots** of wave statistics over time
- 🧭 Visualize **directional trends** using polar plots

---

## 🧑‍🏫 For Students

This notebook is designed to support **learning through exploration**.  
Each code block is clearly explained and marked where user input is expected.  

The notebook runs best on **Google Colaboratory** and saves output to your **Google Drive**.

---

## 📁 Structure

```
wave_analysis/
├── Download_waves_Copernicus.ipynb                ← Main analysis notebook
├── output_data/                  ← Exported CSV data
├── output_images/                ← Generated figures
```

---

## 🚀 Getting Started

1. 🔓 **Create an account** on [marine.copernicus.eu](https://marine.copernicus.eu/)
2. ✅ Save your credentials by running the command:
   `copernicusmarine.login()`
3. 🔽 Clone this repository or download it to your **Google Drive**
4. 📍 Open the notebook in **Google Colab**
5. 🗺 Define your **area of interest** and **virtual buoy** location
6. ▶️ Run the notebook step by step

---

## ▶️ Demo Video

COMING SOON!

---

## 📚 Dataset Info

- **Product**: GLOBAL_REANALYSIS_WAV_001_032  
- **Period**: 1993–2023  
- **Resolution**: ~1/5°  
- **DOI**: [10.48670/moi-00022](https://doi.org/10.48670/moi-00022)

Reference:  
*Law-Chune, S., Aouf, L., Dalphinet, A. et al. WAVERYS: a CMEMS global wave reanalysis. Ocean Dyn 71, 357–378 (2021).*

---

## 📝 Acknowledgments

This notebook was developed by **Alessio Rovere** at **Ca' Foscari University of Venice**,  
with the support of **ChatGPT by OpenAI** for code organization and documentation.

This work is part of the **WARMCOASTS** project, funded by the **European Research Council (ERC)**  
under the European Union’s Horizon 2020 programme (grant agreement n. **802414**).

> ⚠️ **Disclaimer**:  
> Code is provided as-is. Users must validate outputs and adapt it to their research.  
> Neither the authors nor the EU are liable for any outcomes derived from this tool.
