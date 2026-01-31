# Lotka–Volterra Predator–Prey Simulation  
## Numerical Analysis of Ecological Population Dynamics

---

## System Overview
This project implements the **Lotka–Volterra predator–prey model** to simulate interactions between a predator population (cheetah) and a prey population (antelope). The system compares two numerical integration schemes to study population dynamics, numerical stability, and error behavior.

The simulation highlights oscillatory population behavior and evaluates the accuracy of different time-integration methods.

---

## High-Level Architecture

### Mathematical Model Layer
**State Variables:**
- a(t): Prey (antelope) population  
- c(t): Predator (cheetah) population  

**Model Parameters:**
- $$\( k_a = 1.0 \)$$ : Prey birth rate  
- $$\( k_{ca} = 1.0 \)$$: Predator–prey interaction rate  
- $$\( k_c = 0.5 \)$$ : Predator death rate  
- $$\( k_{ac} = 0.5 \)$$ : Predator growth rate  

The coupled nonlinear differential equations govern population evolution over time.

---

### Numerical Integration Layer
**Methods Implemented:**
- Explicit Euler Method  
- Runge–Kutta Method (Second Order, RK2)  

**Comparison Focus:**
- Stability  
- Accuracy  
- Error growth with time step size  

---

### Simulation Layer
- Discrete-time simulation over fixed time intervals  
- Iterative update of predator and prey populations  
- Configurable time step for convergence analysis  

---

### Visualization Layer
- Time-series plots showing population evolution  
- Phase-space plots illustrating predator–prey cycles  
- Log-log plots for numerical error analysis  

---

## Execution Flow
1. Define Lotka–Volterra system parameters  
2. Initialize predator and prey populations  
3. Integrate equations using Explicit Euler method  
4. Integrate equations using RK2 method  
5. Compare population trajectories  
6. Compute numerical error metrics  
7. Visualize results using time-series, phase, and log-log plots  

---

## Results & Insights
- Predator and prey populations exhibit periodic oscillations  
- RK2 provides improved stability and lower numerical error compared to Euler  
- Smaller time steps reduce numerical artifacts  
- Phase plots clearly demonstrate cyclic ecological behavior  

---

## Bug Fixes & Improvements
- Fixed invalid import statements  
- Corrected NumPy alias usage for consistency  
- Improved performance by optimizing array appends  
- Reduced redundant computations in error calculation routines  

---

## Scalability & Extensibility
- Extendable to higher-order Runge–Kutta methods  
- Can incorporate stochastic effects or noise  
- Adaptable to multi-species ecological models  
- Suitable for numerical method benchmarking  

---

## Applications
- Ecological and population dynamics modeling  
- Numerical methods comparison and validation  
- Computational science education  
- Simulation-based analysis of nonlinear systems  

---

## License
MIT License. Free to use, modify, and distribute for academic and research purposes.
