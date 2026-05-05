## 🏛️ System Architecture

<img width="630" height="514" alt="image" src="https://github.com/user-attachments/assets/d3b989c3-2b81-4bec-8579-ebcde43fc5d3" />


### Architecture Overview
Household HQ utilizes a **Multi-Agent Architecture (Option B)** integrated with a **Deep Learning Temporal Forecast** engine. 

* **LSTM Model (The Analyst):** The core deep learning component. It processes "State Check" and "Local" transaction history as a 3D Tensor to predict future liquidity.
* **Lead Financial Steward (The Auditor):** A CrewAI agent that uses RAG (Retrieval-Augmented Generation) to verify fixed obligations against the `Budget.csv`.
* **Strategic Scheduler (The Planner):** A CrewAI agent that interprets the LSTM's 30-day forecast to identify "troughs" and automate the financial roadmap.

