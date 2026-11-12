# Mars Habitability: Statistical Analysis

Statistical investigation into whether humanity can survive and live on Mars based on planetary, atmospheric, and environmental data

## Project Structure
- `data/` — Raw and cleaned datasets used for the analysis
- `mars-habitability-stats.ipynb` — Jupyter Notebook containing data preprocessing, statistical tests, and visualizations
- `mars-habitability-stats_presentation.pdf` — Presentation summarizing the methodology, key metrics, and final conclusions

## Data & Preprocessing
- **Source:** NASA Planetary Data System (PDS) — Mars Reconnaissance Orbiter (MRO), Mars Climate Sounder (MCS) Atmospheric Profiles (`MROM_2001` dataset, [PDS Atmospheres Node](https://atmos.nmsu.edu/PDS/data/MROM_2001/))
- **Cleaning:** Parsed raw NASA `.TAB` data into a structured tabular format, removed redundant telemetry columns, and selected key atmospheric and environmental variables for analysis
## Methods & Tools
- **Language:** Python
- **Libraries:** Pandas, NumPy, Statsmodels, Matplotlib / Seaborn
* **Statistical & Forecasting Techniques:** Time Series Analysis (stationarity testing, decomposition, autocorrelation), ARIMA modeling for atmospheric/environmental forecasting, and descriptive statistics
## Key Findings
1. **Altitude & Temperature:** At lower altitudes (from **-60 meters to -50 meters** relative to the reference datum), ARIMA time series modeling indicates temperatures ranging between **-20°C and -40°C** - significantly milder than average Martian surface extremes
2. **Atmospheric Pressure:** Within this altitude zone, atmospheric pressure reaches approximately **80 kPa**, which is close to Earth-like conditions (~101.3 kPa at sea level) and much higher than the Martian surface average (~0.6 kPa)
3. **Habitability Conclusion:** While unprotected human survival on Mars remains impossible due to sub-zero temperatures and non-breathable atmospheric composition, specific low-altitude/subsurface zones offer favorable pressure and thermal conditions that substantially reduce engineering requirements for pressurized habitats
