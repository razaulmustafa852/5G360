# Mobile 360° Video QoE: Empirical Analysis of 5G QoS Metrics

This repository contains datasets collected from **Operator X** and **Operator Y**, covering **5G radio metrics** and **Quality of Experience (QoE)** for two use cases: **Indoor** and **Mobility**.  
Data was collected at **1-second intervals**.

---

## 📂 Dataset Structure

### 🔹 Indoor Use Case
- **Operator X**
  - `operator-x.csv` → 5G radio metrics  
  - `operator-x-QoE-V1.csv` → corresponding QoE logs  

- **Operator Y**
  - `operator-y.csv` → 5G radio metrics  
  - `operator-y-QoE-V1.csv` → corresponding QoE logs  

### 🔹 Mobility Use Case
- `mobility-x-y.csv` → 5G radio metrics (combined Operator X & Y)  
- `mobility-x-y-QoE-V1.csv` → corresponding QoE logs  

---

## 🔑 Experiment Details

- **Indoor:**  
  Separate files for Operator X and Operator Y.  

- **Mobility:**  
  - Total experiments: **25**  
    - **10** with Operator X  
    - **15** with Operator Y  
  - All experiments stored in `mobility-x-y.csv`  

---

## 🔗 Linking Metrics and QoE

- Each experiment in the metrics file (`*.csv`) is uniquely identified by the column **`SourceFile`**.  
- The corresponding QoE file uses the column **`Eid`** to link records.  

**Example:**  
- If `SourceFile = "10id"` in `operator-x.csv`,  
- Then QoE logs will be found in `operator-x-QoE-V1.csv` under `Eid = "10id"`.  

This mapping applies to both **Operator X** and **Operator Y** datasets.  

---

## 📊 Summary

- **Metrics files (`*.csv`)** → 5G radio network data  
- **QoE files (`*-QoE-V1.csv`)** → corresponding QoE logs  
- Supports **Indoor** and **Mobility** use cases with experiment-level linking  

---
