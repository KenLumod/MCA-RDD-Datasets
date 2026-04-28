# ENHANCED COMPUTATIONAL MODELING OF URBAN EVACUATION: Reverse Dynamic Dijkstra-Based Routing and Hazard Penalty Simulation in Mesoscopic Cellular Automata

##  Overview
This repository contains the map datasets used in the study:

**“ENHANCED COMPUTATIONAL MODELING OF URBAN EVACUATION:  
A REVERSE DYNAMIC DIJKSTRA-BASED ROUTING AND HAZARD PENALTY-BASED SIMULATION IN MESOSCOPIC CELLULAR AUTOMATA.”**

The datasets represent real-world environments transformed into mesoscopic structures for evacuation simulation.

---

##  Data Source and Processing

- Source: **OpenStreetMap (OSM)**
- Processing Tool: **QGIS**
- Workflow:
  1. Extract map data from OpenStreetMap
  2. Clean and filter relevant spatial features
  3. Retain only traversable areas (roads, walkways, paths)
  4. Remove non-traversable regions (buildings, restricted areas, open fields)
  5. Convert into mesoscopic road-cell network

---

## 📊 Dataset Coverage

###  Primary Datasets (Used in Results)
- USTP Cagayan de Oro Campus  
- USEP Campus  
- Gusa Capistrano Complex (CapCom)  

### ⚙️ Supplementary Datasets (Testing Only)
- Barbara Map, Kauswagan, Cagayan de Oro  
- Caraga State University Campus  

> Note: Supplementary datasets were used for model testing and validation but are **not included in the final experimental results**.

---

##  Data Structure

Each map dataset is transformed into a **mesoscopic road-cell network**, where:

- Each cell represents approximately **10m × 6m**
- Only **walkable paths** are included
- Buildings act as **source-loading zones**
- The network forms a **connected graph structure**

### Key Components:
- Road cells (mesoscopic units)
- Cell adjacency / connectivity
- Exit points (evacuation destinations)
- Source/loading regions (starting points of evacuees)

---

##  Purpose of the Dataset

These datasets serve as the **foundation of the simulation model**, enabling:

- Reverse Dynamic Dijkstra (RDD) routing
- Hazard-aware evacuation modeling
- Congestion and flow simulation
- Fire and smoke propagation analysis

The datasets are specifically designed for use within a  
**Mesoscopic Cellular Automata (MCA) framework**.
