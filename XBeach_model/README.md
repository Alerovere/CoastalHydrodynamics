
# 🛠️ XBeach Preprocessing Tool – Bathymetry, Forcing, and Model Setup

This repository provides a modular, student-friendly notebook to **prepare and enhance an XBeach model** using Python in Google Colaboratory.

The script is designed to support **educational and research applications** by guiding users through the key preprocessing steps required before running XBeach — including grid validation, non-erodible mask creation, wave and tide file formatting, and dynamic updates to the `params.txt` file.

> 🌐 Fully compatible with **Google Colaboratory**, with automatic Google Drive integration for file input and output.

🎬 *YouTube tutorial coming soon*

---

## 🚀 Features

- 📁 Automatically mounts your **Google Drive** and organizes your working directory
- 🗺️ Loads and visualizes the **XBeach computational grid** (`x.grd`, `y.grd`, `bed.dep`)
- 🧱 Allows users to upload a **GeoJSON mask** and rasterize it as a non-erodible `.dep` file
- 🌊 Generates `manning_layer.dep` from a roughness GeoJSON (with spatially variable Manning's n)
- 🔄 Updates `params.txt` to include external layers and adapt wave model configuration
- 🌡️ Imports wave time series (`Waves.csv`) and converts it to `jonswap.txt` for instationary wave forcing
- 🕓 Automatically sets simulation timing (`tstart`, `tstop`, `tintg`, `tintm`) based on wave duration
- 🌍 Adds **sea-level rise offsets** to `tide.txt` using constant elevation shifts
- 📋 Validates and prints final `params.txt` for inspection before running XBeach

---

## 📁 Example Directory Layout

```
XBeach_Model/
├── XBeach_preprocessing.ipynb          ← Main setup and preprocessing notebook
├── Model/
│   ├── GeoJson_INPUT/
│   │   ├── Non_erodible.geojson
│   │   ├── manning_roughness.geojson
│   ├── Wave_input/
│   │   ├── Waves.csv
```

---

## 🧪 How to Use It (Google Colab)

This notebook is intended to run in **Google Colaboratory**, connected to your **Google Drive**.

### 🧭 Step-by-step:

1. **Download or clone this repository**
2. **Upload the folder to Google Drive**  
   Suggested path: `My Drive/CoastalHydrodynamics/XBeach_Model/`
3. **Open the notebook with Google Colaboratory**
4. **Follow the notebook cells step by step**:
   - Mount Drive and set working directory
   - Load and validate grid and input files
   - Create or upload GeoJSON masks
   - Format wave and tide input files
   - Adjust model parameters and export outputs

> ✅ All outputs are written back to the model folder, ready to run with XBeach

---

## 📊 Sea-Level Rise Input (Optional)

To add sea-level rise, the notebook modifies `tide.txt` by applying a constant vertical offset to water levels. You can obtain projected sea-level values from:

🌐 [NASA IPCC AR6 Sea Level Projection Tool](https://sealevel.nasa.gov/ipcc-ar6-sea-level-projection-tool)

---

## 📦 Dependencies

Works out of the box with **Google Colab**. Uses:

- `numpy`, `pandas`, `matplotlib`, `seaborn`, `xarray`
- `geopandas`, `shapely`, `tqdm`
- `rasterio` (for spatial file handling)

---

## 📝 Acknowledgments

Developed by **Alessio Rovere** at **Ca' Foscari University of Venice**, with scripting support and documentation assistance from **ChatGPT by OpenAI**.

Part of the **WARMCOASTS** project, funded by the **European Research Council (ERC)** under grant agreement n. **802414**.

> ⚠️ Disclaimer: This code is intended for educational and research use. Users are responsible for verifying results before operational use.

---

## 📬 Contact

For questions, improvements, or reporting issues, please open a GitHub Issue or contact the project maintainer directly.


---

## 🌐 External Tools Required

To run XBeach simulations, you will need to install the following tools locally:

- 🧰 **Delft Dashboard** – for building the initial XBeach model grid and input files  
  🔗 [https://publicwiki.deltares.nl/spaces/DDB/pages/77234207/Download](https://publicwiki.deltares.nl/spaces/DDB/pages/77234207/Download)

- 🌊 **XBeach** – the simulation engine  
  🔗 [https://download.deltares.nl/xbeach](https://download.deltares.nl/xbeach)

---

## 📦 Note on Input Folder Structure

This script assumes that the `Model/` folder already contains a complete set of XBeach input files **exported from Delft Dashboard**. These include:

- `x.grd`, `y.grd`, `bed.dep`, `params.txt`, `tide.txt`, etc.

> 📹 For a step-by-step guide to creating the initial model with Delft Dashboard, see:  
👉 [https://www.youtube.com/watch?v=SgE-CFRTjB8](https://www.youtube.com/watch?v=SgE-CFRTjB8)
