# Axion Emissivity Tables

This repository provides emissivity and absorption tables for axion production in electron relativistic plasma through the following processes:

- Semi-Compton scattering
- Pair annihilation
- Electron-nucleus bremsstrahlung
- Electron-positron coalescence

### **Contents**
The `.dat` files contain:
- **Emissivities** [MeV⁻¹ s⁻¹ cm⁻³]
- **Absorption rates** [s⁻¹]

as a function of:
- Axion mass **m_a** [MeV]
- Axion energy **E_a** [MeV]
- Plasma temperature **T** [MeV]
- Electron plasma chemical potential **mu_e** [MeV]


### **Grid ranges**
| Parameter | Points | Range |
|-----------|--------|-------|
| m_a       | 37     | 0.1 – 1000 MeV |
| E_a       | 131    | 0.1 – 3000 MeV |
| T         | 28     | 1 – 100 MeV |
| mu_e      | 27     | 10 – 500 MeV |

### **Data ordering**
Each `.dat` file has columns: `m_a  E_a  T  mu_e  value`.

A Python notebook **`read_tables.ipynb`** is included to load, interpolate, and visualize the data.
