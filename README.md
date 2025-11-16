# QuantumWaveletShrinkage
Jupyter notebooks with Qiskit 2.x Examples in Quantum Wavelet Shrinkage
# 🧠 Quantum Wavelet Shrinkage

This repository accompanies the research paper  
**“Quantum Wavelet Shrinkage”** by *Brani Vidakovic (Texas A&M University)*.

It demonstrates how classical wavelet denoising can be formulated and implemented in the **quantum domain**, using controlled decoherence, ancilla-driven channels, and expectation-value encoding to realize shrinkage operations on quantum states.  

All examples are written in **Qiskit 2.x** and can be executed locally or on IBM Quantum backends.

---

## 📂 Contents

| Notebook | Description |
|-----------|--------------|
| **QThreshold13.ipynb** | Basic Helstrom-based quantum thresholding with measurement-driven denoising. |
| **QThreshold16a.ipynb** | Phase-damping shrinkage using Kraus and hardware-realizable channels (`T₂` and random Pauli-Z). |
| *(more notebooks forthcoming)* | Demonstrations of channel-based and ancilla-driven shrinkage methods. |

All notebooks are executable and annotated for instructional use.  
They can also be viewed online through **nbviewer** or **Google Colab**.

---

## 🧩 Environment Setup (Anaconda + Jupyter + Qiskit 2.x)

To reproduce the notebooks locally:

### 1️⃣  Create and activate an environment
```bash
conda create -n qiskit2 python=3.10
conda activate qiskit2
