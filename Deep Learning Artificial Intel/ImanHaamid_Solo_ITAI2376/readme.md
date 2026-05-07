# ImanHaamid_Solo_ITAI2376

## 🏛️ System Architecture - Neural Steward: Highlights the LSTM (Neural) and the Agent (Steward)
ITAI 2376 Final Project: Build Your AI Agent - CrewAI-Financial-Agent


### Architecture Overview
Household HQ utilizes a **Multi-Agent Architecture (Option B)** integrated with a **Deep Learning Temporal Forecast** engine. 

* **LSTM Model (The Analyst):** The core deep learning component. It processes "State Check" and "Local" transaction history as a 3D Tensor to predict future liquidity.
* **Lead Financial Steward (The Auditor):** A CrewAI agent that uses RAG (Retrieval-Augmented Generation) to verify fixed obligations against the `Budget.csv`.
* **Strategic Scheduler (The Planner):** A CrewAI agent that interprets the LSTM's 30-day forecast to identify "troughs" and automate the financial roadmap.

---

## 📁 Repository Layout

```
ImanHaamid_Solo_ITAI2376/
├── README.md                          # Project documentation and overview
├── REFLECTION.md                      # Reflection document
├── LICENSE                            # Apache 2.0 License
├── .gitignore                         # Git ignore file
│
├── Notebook/                          # Jupyter Notebooks for development and analysis
│   ├── [Model training and evaluation notebooks]
│   └── [Data processing and EDA notebooks]
│
└── Docs/                              # Documentation and resources
    ├── [Architecture diagrams]
    ├── [API documentation]
    └── [Setup guides]
```

### Directory Descriptions

| Directory | Purpose |
|-----------|---------|
| **Notebook/** | Contains Jupyter Notebooks for LSTM model training, agent development, testing, and data exploration |
| **Docs/** | Project documentation including architecture details, setup instructions, and usage guides |
| **Root Files** | Configuration and metadata files (README.md, LICENSE, .gitignore) |

### Key Files

- **README.md** - Main project documentation
- **LICENSE** - Apache 2.0 License
- **.gitignore** - Git configuration for ignoring local files

---

## 🚀 Demo Video

[ImanHaamid Demo Youtube Video](https://youtu.be/8HDv8wkGdBs)

## 📚 Documentation
[Reflection](REFLECTION.md)

[Docs/Updated_Blueprint_ImanHaamid_Solo_ITAI2376.pdf](Docs/ImanHaamid_Solo_ITAI2376.pdf)

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
