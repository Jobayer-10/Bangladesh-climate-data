🌦️ Bangladesh District-wise Climate Data (2011–2025)

This repository contains historical climate and environmental data for **64 districts of Bangladesh**, covering the period from **2011 to 2025**. Each district has its own `.csv` file with monthly and annual averages for five key parameters.

---

## 📡 Data Source

All data in this repository was retrieved from the **NASA POWER Data Access Viewer**:

🔗 [https://power.larc.nasa.gov/data-access-viewer/](https://power.larc.nasa.gov/data-access-viewer/)

NASA POWER (Prediction Of Worldwide Energy Resources) provides satellite-derived meteorological and solar energy data for research and applications.

---

## 📁 Repository Structure


Each file is named after the district it represents (e.g., `Satkhira.csv`, `Dhaka.csv`).

---

## 📊 Parameters

Each CSV file contains data for the following **5 parameters**:

| Parameter Code | Full Name | Unit |
|---|---|---|
| `ALLSKY_SFC_SW_DWN` | All Sky Surface Shortwave Downward Irradiance | MJ/m²/day |
| `GWETROOT` | Root Zone Soil Wetness (surface to 100 cm depth) | Fraction (0–1) |
| `PRECTOTCORR` | Precipitation (rain, snow, etc.) | mm/day |
| `RH2M` | Relative Humidity at 2 Meters | % |
| `T2M` | Temperature at 2 Meters | °C |

> **Note:** A value of `-999` indicates missing or unavailable data for that month.

---

## 🗂️ CSV File Format

Each CSV file is structured as follows:

- **Rows:** One row per parameter per year
- **Columns:** `PARAMETER`, `YEAR`, `JAN`, `FEB`, `MAR`, `APR`, `MAY`, `JUN`, `JUL`, `AUG`, `SEP`, `OCT`, `NOV`, `DEC`, `ANN`
- `ANN` = Annual average/total

**Example (Satkhira.csv):**

```
PARAMETER,YEAR,JAN,FEB,MAR,APR,MAY,JUN,JUL,AUG,SEP,OCT,NOV,DEC,ANN
ALLSKY_SFC_SW_DWN,2011,13.87,17.7,19.47,20.96,19.88,14.45,16.51,13.7,14.58,17.22,15.38,12.52,16.34
GWETROOT,2011,0.65,0.6,0.59,0.62,0.7,0.81,0.98,0.98,0.99,0.87,0.7,0.61,0.76
PRECTOTCORR,2011,0.01,0.06,1.01,2.13,5.85,11.47,9.88,17.19,9.4,1.23,0.06,0.21,4.9
RH2M,2011,62.22,46.99,50.75,63.43,76.27,84.9,88.09,91.2,91.13,82.08,71.56,64.59,72.92
T2M,2011,17.63,23.2,28.27,29.56,29.83,29.05,28.28,27.68,27.45,26.74,23.31,19.94,25.92
```

---

## 🕒 Temporal Coverage

- **Start Year:** 2011
- **End Year:** 2025
- **Temporal Resolution:** Monthly & Annual

---

## 🗺️ Spatial Coverage

All 64 districts of Bangladesh are covered. Data points are extracted for each district using GPS coordinates of the district centroid via the NASA POWER API.

---

## 📜 License & Citation

Data is publicly available through NASA POWER. If you use this dataset in research or publications, please cite the original source:

> NASA POWER Project. *POWER Data Access Viewer*. NASA Langley Research Center. Retrieved from https://power.larc.nasa.gov/data-access-viewer/

---

## 🤝 Contributing

If you find any errors or want to extend this dataset, feel free to open an issue or submit a pull request.
