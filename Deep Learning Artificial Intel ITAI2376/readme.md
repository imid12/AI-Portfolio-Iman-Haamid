# Deep Learning & Artificial Intelligence Portfolio

<div align="center">

![Deep Learning Portfolio Badge](https://img.shields.io/badge/Deep%20Learning-AI%20Portfolio-blue?style=for-the-badge&logo=tensorflow&logoColor=white)
![Neural Networks](https://img.shields.io/badge/Neural%20Networks-LSTM%20%26%20Diffusion-red?style=for-the-badge&logo=pytorch&logoColor=white)

**Advanced Deep Learning Projects | Neural Steward | Diffusion Models | Financial AI**

</div>

---

This folder contains deep learning and AI projects from the AI Portfolio of Iman Haamid. It includes Jupyter notebooks, documentation, and code for experiments, labs, and the Neural Steward final project.

## 🚀 Tech Stack

![Python](https://img.shields.io/badge/Python-3.8+-3776ab?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-Latest-ee4c2c?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Latest-ff6f00?style=flat-square&logo=tensorflow&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Lab-f37726?style=flat-square&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?style=flat-square&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit%20Learn-ML-f7931e?style=flat-square&logo=scikit-learn&logoColor=white)

---

## 📊 Portfolio Architecture

```
┌─────────────────────────────────────────────────────┐
│     Deep Learning & AI Portfolio Structure          │
├─────────────────────────────────────────────────────┤
│                                                     │
│  ┌──────────────┐  ┌──────────────┐  ┌───────────┐ │
│  │    CODE      │  │    DOCS      │  │  FINAL    │ │
│  │  (Labs)      │  │  (Reports)   │  │  PROJECT  │ │
│  ├──────────────┤  ├──────────────┤  ├───────────┤ │
│  │ • L05, L08   │  │ • Diffusion  │  │ • Neural  │ │
│  │   L09        │  │ • Deep       │  │   Steward │ │
│  │ • Module 02  │  │   Thinkers   │  │ • LSTM +  │ │
│  │   Module 03  │  │ • Reports    │  │   Agents  │ │
│  └──────────────┘  └──────────────┘  └───────────┘ │
│         │                  │                 │      │
│         └──────────────────┴─────────────────┘      │
│                     │                               │
│        🤖 LSTM Neural Networks 🤖                  │
│        📈 Agent-Based Modeling 📈                  │
│        💰 Financial Forecasting 💰                 │
│                                                     │
└─────────────────────────────────────────────────────┘
```

## 📁 Project Structure

```
Deep Learning Artificial Intel/
├── README.md — this file
├── Code/ — Jupyter notebooks for course labs and experiments
│   ├── L05_Iman_Haamid_ITAI2376.ipynb — Lab 5 assignment
│   ├── L08_Diffusion_ImanHaamid_ITAI_2376.ipynb — Lab 8: Diffusion models
│   ├── L09_ImanHaamid_ITAI_2376.ipynb — Lab 9 assignment
│   ├── Module_02_Lab_Iman_Haamid.ipynb — Module 2 lab work
│   └── Module_03_Lab_ImanHaamid.ipynb — Module 3 lab work
│
├── Docs/ — Documentation, reports, and reference materials
│   ├── A02_Deepthinkers_Sha'RiseGriggs_ITAI2376-1.pdf — DeepThinkers assignment
│   ├── A03_DeepThinkers_ShariseGriggs_ITAI2376_pptx.pptx — DeepThinkers presentation
│   ├── A04_DeepThinkers_Andre_Ellis (1).pdf — DeepThinkers contribution
│   └── L08_Diffusion_ImanHaamid_ITAI_2376-1.pdf — Diffusion lab report
│
└── ImanHaamid_Solo_ITAI2376/ — Final Project: Neural Steward
    ├── README.md — Project overview
    ├── LICENSE — Project license
    ├── REFLECTION.md — Project reflection and learnings
    ├── .gitignore — Git configuration
    │
    ├── Notebook/ — Main project notebook
    │   └── ImanHaamid_Solo_ITAI2376.ipynb — Neural Steward implementation
    │
    └── Docs/ — Project documentation and data
        ├── ImanHaamid_Solo_ITAI2376.pdf — Project report
        ├── Historical Spending - transactions.csv — Dataset
        └── requirements.txt — Project dependencies
```

## 📚 Overview of Contents

### Code/
Jupyter notebooks containing course assignments and lab work:
- **L05, L08, L09**: Lab assignments from course ITAI2376
- **Module 02, Module 03**: Module-based lab exercises

### Docs/
Supporting documentation including:
- DeepThinkers collaborative project materials (reports and presentations)
- Detailed lab reports, particularly for the diffusion models assignment

### ImanHaamid_Solo_ITAI2376/ - Neural Steward Final Project
The capstone project combining LSTM neural networks with agent-based modeling for financial forecasting and decision-making.

**Key Files:**
- `Notebook/ImanHaamid_Solo_ITAI2376.ipynb` — Main implementation
- `Docs/ImanHaamid_Solo_ITAI2376.pdf` — Comprehensive project report
- `Docs/Historical Spending - transactions.csv` — Training dataset
- `REFLECTION.md` — Project insights and learnings

## ⚙️ Setup & Requirements

### Environment Setup
A typical environment to run the examples in this folder requires:

- Python 3.8+
- pip or conda
- Key packages:
  - numpy
  - pandas
  - matplotlib
  - jupyter lab / notebook
  - torch / tensorflow
  - scikit-learn
  - tqdm

**Example (venv + pip):**
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
# Or install common packages:
pip install numpy pandas matplotlib scikit-learn torch torchvision jupyterlab tqdm
```

**Example (conda):**
```bash
conda create -n deeplearning python=3.9
conda activate deeplearning
pip install -r requirements.txt
```

### For the Final Project
See `ImanHaamid_Solo_ITAI2376/Docs/requirements.txt` for project-specific dependencies.

## 🏃 Running the Notebooks

1. Activate your virtual environment
2. Start Jupyter Lab:
   ```bash
   jupyter lab
   ```
3. Navigate to and open any `.ipynb` file in the `Code/` or `ImanHaamid_Solo_ITAI2376/Notebook/` directories

## 🤝 Contributing

To contribute or add new experiments:
1. Create a new notebook or folder under `Code/`
2. Include a clear description of the experiment or lab work
3. Add dependencies to `requirements.txt`
4. Open a pull request with a summary of changes

## 📧 Contact

- **Author:** Iman Haamid
- **GitHub:** [@imid12](https://github.com/imid12)
- **Repository:** [AI-Portfolio-Iman-Haamid](https://github.com/imid12/AI-Portfolio-Iman-Haamid)

---

<div align="center">

**Made with ❤️ for Deep Learning Research & Development**

</div>
