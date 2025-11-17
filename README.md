# 🧠 Quantum Wavelet Shrinkage

This repository accompanies the research paper  
**“Quantum Wavelet Shrinkage”** by *Brani Vidakovic (Texas A&M University)*.

It demonstrates how classical wavelet denoising can be formulated and implemented in the **quantum domain**, using controlled decoherence, ancilla-driven channels, and expectation-value encoding to realize shrinkage operations on quantum states.  

All examples are written in **Qiskit 2.x** and can be executed locally or on IBM Quantum backends.

---

## 📂 Contents

| Notebook | Description |
|-----------|--------------|
| **QWShrink01.ipynb** | Applies DAUB2 8x8 for 3 cubits as a single gate and compares the results with classical approaces.  |
| **QWShrink02.ipynb** | Quantum Haar Wavelet Transform (3 levels) via factorized circuit Hadamards + (zero-)controlled Hadamards|
| **QWShrink03.ipynb** | Quantum expectation and Kraus phase damping with data dependent strength|
| **QWShrink04.ipynb** | Phase-damping shrinkage using Kraus and hardware-realizable channels |
| **QWShrink05.ipynb** | Basic Helstrom-based quantum thresholding with measurement-driven   |
| **QWShrink06.ipynb** | Phase-damping shrinkage using Kraus and hardware-realizable channels |
| **QWShrink07.ipynb** | Basic Helstrom-based quantum thresholding with measurement-driven   |
| **QWShrink08.ipynb** | Phase-damping shrinkage using Kraus and hardware-realizable channels |
| **QWShrink09.ipynb** | Basic Helstrom-based quantum thresholding with measurement-driven   |
| **QWShrink10.ipynb** | Phase-damping shrinkage using Kraus and hardware-realizable channels |
| **QWShrink11.ipynb** | Basic Helstrom-based quantum thresholding with measurement-driven   |



All notebooks are executable and annotated for instructional use.  
They can also be viewed online through **nbviewer** or **Google Colab**.

---

## 🧩 Environment Setup (Anaconda + Jupyter + Qiskit 2.x)

To reproduce the notebooks locally:

### 1️⃣  Create and activate an environment
```bash
conda create -n qiskit2 python=3.10
conda activate qiskit2
```

### 2️⃣  Install Jupyter
```bash
conda install jupyterlab
# or
conda install notebook
```

### 3️⃣  Install Qiskit 2.x and dependencies
```bash
pip install qiskit==2.*
pip install qiskit[visualization]
```

### 4️⃣  Add supporting libraries
```bash
pip install numpy matplotlib seaborn pylatexenc ipywidgets
```

### 5️⃣  Register the kernel for Jupyter
```bash
python -m ipykernel install --user --name qiskit2 --display-name "Qiskit 2.x"
```

### 6️⃣  Launch Jupyter
```bash
jupyter lab
# or
jupyter notebook
```
In Jupyter, choose **Kernel → Change Kernel → Qiskit 2.x**.

---

## ✅ Quick Test
```python
from qiskit import QuantumCircuit
qc = QuantumCircuit(2)
qc.h(0)
qc.cx(0, 1)
qc.draw('mpl')
```
If you see the circuit diagram, your installation works correctly.

---

## ⚙️ Optional Extras

- **Aer simulator** (faster local simulation)
  ```bash
  pip install qiskit-aer
  ```
- **IBM Runtime** (real-hardware execution)
  ```bash
  pip install qiskit-ibm-runtime
  ```

---

## 📘 Reproducibility and Citation

All notebooks are compatible with **Qiskit 2.x** and **Python 3.10**.  
They are designed for clarity and reproducibility in both research and teaching.  

If you use these materials, please cite:

> B. Vidakovic, *Quantum Wavelet Shrinkage*, Texas A&M University, 2025.

---

*Author — Brani Vidakovic*  
*Department of Statistics, Texas A&M University*

