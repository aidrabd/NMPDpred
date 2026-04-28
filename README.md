# NMPDpred (Neuroinflammation mediated Parkinson's Disease Prediction)
A **Machine Learning–Aided Compounds Screening Tool** for predicting pIC₅₀ against MMP9**.  

---

## 🚀 Key Applications
- **Compounds Screening:** Identify compounds against neuroinflammatory target MMP9  
- **Virtual Screening:** Rapidly assess compound libraries with inhibition potential  
- **Lead Optimization:** Predict activity and guide structural modifications  
- **Decision Support:** Prioritize candidates for *in vitro* and *in vivo* testing  

---

## 📊 Model Performance
Our **Random Forest regression model** demonstrated strong predictive performance with excellent generalization ability:  

| Dataset | R² Score |
|----------|-----------|
| Training Set | 0.8868 |
| Validation Set | 0.7848 |
| Test Set | 0.8061 |
| CV | **0.8116** |

The consistency of R² accross datasets highlight the robustness of the model in predicting inhibitory activity (pIC₅₀) against MMP9.  

---

## ⚙️ Installation

### Prerequisites
- Python ≥ 3.8  
- `conda` package manager  

### Install
### Prerequisites

- Ubuntu/Linux terminal/Window Command Line

### Installation

```bash
# Clone and setup
git clone https://github.com/aidrabd/TarEGFR.git
cd TarEGFR

# Make prediction script executable
chmod +x predict.py
```

First, make sure you have conda installed:

```bash
1. Install  Miniconda (if not installed)

wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh

2. Activate conda base environment

Type "conda init"

Then, restart your terminal

After that, activate the base environment with:

conda activate
```

Second, make sure you have Python specific version installed:

```bash
conda create -n py312 python=3.12.9
conda activate py312
python --version
```

---

## 🏃‍♂️ Simple Start

### Command Line Usage
```bash
python predict.py
# Provide input file name (e.g., sample.csv)
# Columns required in File: SMILES, pIC50 (Leave pIC50 empty for prediction)
```

### 🧾 Input Format
| Column | Description |
|---------|--------------|
| **SMILES** | Simplified Molecular Input Line Entry System notation |
| **pIC50** | Predicted biological activity (keep empty for prediction) |
# See sample.csv file to prepare your own file.

---

## ⚠️ Disclaimer
**NMPDpred** is developed for **research purposes only**.  
All predictions should be validated experimentally before any clinical or commercial application.  

---

## 📄 License
This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.  

---

## 📚 Citation
If you use **NMPDpred** in your research, please cite:  

---

## 🙏 Acknowledgments
- Training data curated from **ChEMBL** and published literature  
- Molecular descriptors generated using **RDKit**  
- Molecular docking and dynamics simulations performed using **AutoDock Vina** and **Schrodinger's DESMOND**  
- Special thanks to the **open-source bioinformatics and cheminformatics communities**
