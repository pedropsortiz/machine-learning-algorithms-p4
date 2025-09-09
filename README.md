
# Machine Learning Algorithms P4

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![P4](https://img.shields.io/badge/P4--lang-Network%20Programming-orange)](https://p4.org/)

This repository presents the integration of **Machine Learning algorithms** with **P4 (Programming Protocol-Independent Packet Processors)**, aiming to explore applications of **intelligent programmable networks**.  

The goal is to demonstrate how machine learning models can be used for traffic classification, packet prioritization, and real-time analysis inside programmable switches.

---

## Features
- Implementation of ML algorithms (KNN, Linear Regression, Decision Trees).  
- Training and validation in Python.  
- Export of trained models for use in **P4 pipelines**.  
- Simulation environment using **Mininet**.  
- Scripts for dataset generation and performance evaluation.  

---

## Requirements
- **Operating System:** Linux (Ubuntu/Mint recommended)  
- **Main dependencies:**  
  - [Python 3.9+](https://www.python.org/)  
  - [Mininet](http://mininet.org/)  
  - [P4C Compiler](https://github.com/p4lang/p4c)  
  - [Scapy](https://scapy.net/)  

- **Python libraries:**  
  ```bash
  pip install numpy pandas scikit-learn matplotlib jupyter
## Repository Structure

```
machine-learning-algorithms-p4/
│── p4/                  # P4 programs used in experiments
│── python/              # ML algorithms in Python
│   ├── models/          # Trained models
│   ├── datasets/        # Datasets
│   └── scr/         # Training and testing scripts
│── notebooks/           # Jupyter Notebooks with analysis
│── results/             # Results and metrics
│── README.md            # Main documentation
```

---

## How to Run

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/machine-learning-algorithms-p4.git
   cd machine-learning-algorithms-p4
   ```

2. **Compile and run the P4 program**

   ```bash
   sudo p4run --config p4/config.json
   ```

3. **Train a Machine Learning model**

   ```bash
   cd python/scripts
   python train_knn.py
   ```

4. **Validate integration with network packets**

   ```bash
   sudo python test_packets.py
   ```

---

## Example Applications

* **Packet classification:** HTTP vs HTTPS with KNN.
* **Metric prediction:** Network latency using Linear Regression.
* **Intelligent management:** Dynamic traffic prioritization with Decision Trees.

---

## Resources and References

* [Official P4 Documentation](https://p4.org/)
* [Mininet - Network Emulator](http://mininet.org/)
* [Scikit-Learn - ML in Python](https://scikit-learn.org/)

---
