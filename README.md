# 📱 Mobile 360° Video QoE: Empirical Analysis of 5G QoS Metrics

This repository contains datasets collected from **Operator X** and **Operator Y**, covering **5G radio metrics** and **Quality of Experience (QoE)** for two use cases: **Indoor** and **Mobility**.  
Data was collected at **1-second intervals**.

---

## 📂 Dataset Structure

### 🔹 Indoor Use Case
| Operator | 5G Metrics File | QoE File |
|-----------|------------------|----------|
| X | `operator-x.csv` | `operator-x-QoE.csv` |
| Y | `operator-y.csv` | `operator-y-QoE.csv` |

### 🔹 Mobility Use Case
| File | Description |
|-------|--------------|
| `mobility-x.csv` | 5G radio metrics (Operator X) |
| `mobility-x-QoE.csv` | Corresponding QoE logs |
| `mobility-y.csv` | 5G radio metrics (Operator Y) |
| `mobility-y-QoE.csv` | Corresponding QoE logs |

---

## 🔑 Experiment Details

- **Indoor:**  
  Separate experiment files are available for **Operator X** and **Operator Y**.

- **Mobility:**  
  - Total experiments: **25**  
    - **10** with Operator X  
    - **15** with Operator Y  
  - All experiments are stored in `mobility-x.csv` and `mobility-y.csv` with their corresponding QoE in `mobility-x-QoE.csv` and `mobility-y-QoE.csv`

---

## 🔗 Linking 5G Metrics and QoE

Each record in the datasets is associated with an **`experiment`** number.  
This column uniquely identifies experiments across both the **5G metrics** and **QoE** files.

**Example:**
If experiment = 3 in mobility-x.csv  
Then the corresponding QoE logs can be found in mobility-x-QoE.csv where experiment = 3

## 🧠 Citation

If you use this dataset, please cite the following paper:

> **Raza Ul Mustafa**  
> *Mobile 360° Video QoE: Empirical Analysis of 5G QoS Metrics*  
> In *Proceedings of the 28th International Conference on Modeling, Analysis and Simulation of Wireless and Mobile Systems (MSWiM 2025)*,  
> **Barcelona, Spain**, 2025.

---

### 📄 BibTeX
For convenience, you can cite this work using the following BibTeX entry:

```bibtex
@inproceedings{mustafa2025mobile360,
  author    = {Raza Ul Mustafa},
  title     = {Mobile 360° Video QoE: Empirical Analysis of 5G QoS Metrics},
  booktitle = {Proceedings of the 28th International Conference on Modeling, Analysis and Simulation of Wireless and Mobile Systems (MSWiM 2025)},
  year      = {2025},
  address   = {Barcelona, Spain}
}
