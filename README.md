# battery_projects
working with publicly available battery data

## Li-ion Arbin.ipynb

### Summary
* Tests of 3 different batteries at different temperatures and C-rates.
* Have "record data": time, current, voltage, temperature.
* Only 1 cycle per test available in this dataset. 

### About the data in this notebook:
* Data downloaded from: https://data.mendeley.com/datasets/kxsbr4x3j2/2 (on 17/05/2025)
* stored and unzipped locally
* Original article: https://www.sciencedirect.com/science/article/pii/S2352340921001785?via%3Dihub
* Data generated with an Arbin tester and its associated software, MITS Pro-software and Data Watcher

### Work done:

(to be updated for each version of the notebook)

* Initial EDA
* Some data engineering for the record data, e.g. dQ, dV

### to do:
* plots with the record data:
  * V and I vs t, including overlays of relevant combinations of tests (usually would do this for different cycles with the same device, e.g. at the beginning and end of the cycling testing, will probably do it for different temperatures at the same C-rate here)
  * dQ/dV vs V
* calculate parameters for each step:
  * energy, capacity
* calculate parameters for each cycle:
  * energy efficiency, coulombic efficiency
  * self-discharge (if there is a rest / OCV step between the charge and discharge steps)
