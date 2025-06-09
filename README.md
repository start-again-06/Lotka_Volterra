# 🐆 Lotka-Volterra Predator-Prey Simulation 🦌

## 📌 Overview
This project implements the **Lotka-Volterra model**, which describes the interaction between predator (*cheetah*) and prey (*antelope*) populations. It compares two numerical methods:

- 📍 **Explicit Euler Method**  
- 📍 **Runge-Kutta (RK2) Method**

---

## ✨ Features
✅ Simulates predator-prey dynamics over time  
✅ Numerical integration using Euler and RK2 methods  
✅ Visualizes population evolution with time-series and phase plots  
✅ Error analysis of numerical methods

---

## 📂 Workflow

### 1️⃣ Lotka-Volterra Equations
The system models two species:

- `a(t)`: Prey (antelope) population  
- `c(t)`: Predator (cheetah) population  

Equations:

\[
\frac{da}{dt} = k_a \cdot a - k_{ca} \cdot a \cdot c
\]  
\[
\frac{dc}{dt} = -k_c \cdot c + k_{ac} \cdot a \cdot c
\]

Parameters:

- `k_a = 1.0` → Prey birth rate  
- `k_ca = 1.0` → Predator-prey interaction  
- `k_c = 0.5` → Predator death rate  
- `k_ac = 0.5` → Predator growth rate  

---

### 2️⃣ Numerical Integration Methods

- 🚀 **Explicit Euler**: Basic first-order method, faster but less accurate  
- 🚀 **RK2 (Runge-Kutta 2nd Order)**: More accurate, better stability  

---

### 3️⃣ Simulation & Visualization

- 📊 **Time-Series Plots**: Tracks population changes over time  
- 📉 **Phase Plots**: Visualizes predator-prey cycles  
- 📈 **Log-Log Error Analysis**: Compares integration accuracy  

---

## 📊 Results & Insights

- Predator-prey cycles: The populations oscillate periodically  
- RK2 performs better than Euler, with lower numerical error  
- Higher time steps improve accuracy, reducing numerical artifacts  

---

## 🐞 Bug Fixes & Improvements

- 🚨 Fixed import errors  
  - ✅ Removed `from python import random` (invalid import)  
  - ✅ Used `import numpy as np` correctly  
- 🚨 Performance Optimization  
  - ✅ Used `np.append()` more efficiently in integration  
  - ✅ Reduced redundant calculations in `computeError()`

---

## 🔚 Conclusion

This project models a classic ecological system with robust numerical methods. It provides insights into population dynamics and computational accuracy.

---

## 📜 License

🔓 **MIT License** – Free to use and modify!

