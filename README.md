# ForMap — Urban Thermal Simulation

**ForMap** generates thermal maps of entire cities from open-source geospatial data (OpenStreetMap + Copernicus), by simulating radiative and convective heat exchange in urban street canyons.

**244 000 canyons across Milan — simulated in 46 seconds on a single GPU.**

---

## Interactive outputs — full city

| | |
|---|---|
| [🗺 Thermal map](https://federicomattiuz.github.io/ForMap_Results/map_interactive.html) | All 244 k canyons coloured by peak air temperature |
| [⏱ Hourly animation](https://federicomattiuz.github.io/ForMap_Results/temporal_slider.html) | Temperature snapshots across the day |
| [📊 Canyon shading effect](https://federicomattiuz.github.io/ForMap_Results/canyon_effect.html) | Peak temperature vs canyon aspect ratio H/W |

---

## Climate scenario comparison — Milan, 21 June

Same geometry, different overnight temperature.

| Scenario | T_morning | Mean T_air_max | Canyons > 30 °C |
|---|---|---|---|
| Milan 2024 (recent normal) | 20.1 °C | 25.8 °C | ~4 % |
| **2022 heatwave overnight** | **24.6 °C** | **30.2 °C** | **~50 %** |

**×12.5 more canyons exceed 30 °C** during a heatwave night — the same streets, different climate forcing.

<p align="center">
  <img src="static_maps/milan_2024.png" width="48%" alt="Milan 2024 thermal map"/>
  <img src="static_maps/milan_2022_heatwave.png" width="48%" alt="2022 heatwave thermal map"/>
</p>

*Same colour scale on both maps. Purple/violet = cooler streets. Orange/red = hottest.*

---

## Verify the physics

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/FedericoMattiuz/ForMap_Results/blob/main/notebooks/ForMap_Demo.ipynb)

The notebook runs the same 5-node ODE physics on ~1 100 canyons from Milan's Centrale district (~2 min on free Colab CPU). No GPU or private code needed.

---

*Contact: federico.mattiuz00@gmail.com*
