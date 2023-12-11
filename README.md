# Split Encoding for Data Re-uploading Based Quantum Classifier

Please refer to the [Project Report](https://drive.google.com/file/d/1yk-QxEXgC9KDdUrcfXW12qCLNrnK2VeA/view?usp=sharing) for complete details of the proposed technique. 

# Abstract 
Quantum computers hold a lot of promise for applications in machine learning. In the current
era of noisy intermediate-scale quantum (NISQ) computers, optimizing quantum circuits to work
with as few qubits as possible is highly favorable. Recent advances in hybrid quantum-classical
methods have made it possible to build a classification model based on variation circuits with
as few as one qubit. However, it is still unclear how to choose an effective encoding technique.
This project aims to design an encoding technique to minimize circuit depth while preserving
classification accuracy. Finally, I test the new and existing methods and compare their performance
on real-world datasets. 

# Installation

Install the libraries listed in the requirements.txt file in a Python 3.9+ virtual environment. 

```
  python3 -m venv .venv
  source .venv/bin/activate
  pip install -r requirements.txt
```

## Note on Pennylane Lightning-GPU 

The use of Pennylane's Lightning-GPU plugin is recommended but not required. If a system does not have access to a GPU, Pennylane should fall back to the regular `lightning.qubit` device. In case there are issues, it is sufficient to replace `dev = qml.device("lightning.gpu", ...)` by `dev = qml.device("lightning.qubit", ...)`. 
