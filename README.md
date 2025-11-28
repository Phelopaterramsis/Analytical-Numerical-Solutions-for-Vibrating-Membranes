# 🧮 Analytical & Numerical Solutions for Vibrating Membranes  
A full analytical and numerical study of circular and rectangular vibrating membranes using PDE theory, separation of variables, Bessel functions, Fourier series expansions, and FEATool Multiphysics simulations.

## 📌 Course  
**MATH 302 – Partial Differential Equations (PDEs)**  
Applied Mathematics Department  
University of Science and Technology – Zewail City  
Supervisor: **Prof. Ahmed Abdelsamea**

## 👥 Team  
- **Phelopater Ramsis – 202001171**  
- Yossef Adel – 202001273  
- Hassan Mohamed – 202000932  

---

## 📘 Project Overview  
This project investigates the **vibration behavior of 2D elastic membranes**—a classical PDE problem with deep applications in:

- Acoustics (e.g., drum membranes)  
- Mechanical and civil engineering  
- Waveguides and communication systems  
- Biological membranes (eardrum behavior)  
- Thin-film devices  

The study includes both **analytical solutions** using PDE techniques and **numerical simulations** using FEATool Multiphysics.

---

## 🧠 Mathematical Framework

### **1. Governing Equation**  
The vibration of a membrane is described by the 2D wave equation:

\[
u_{tt} = c^2 (u_{xx} + u_{yy})
\]

where  
- *u(x, y, t)* = membrane displacement  
- *c* = wave propagation constant  

The solution fully depends on geometry + boundary conditions.

---

## 🎯 Solved Cases

### **🔵 1. Circular Membrane**  
Pages 4–8 of the report show the full derivation. The solution uses:

- Separation of variables  
- Bessel’s differential equation  
- Eigenvalue constraints from boundary conditions  
- Zeroes of **Jn(αr)**  
- Orthogonality relations for Fourier–Bessel series  

The final solution is a double infinite series involving:  
- **Bessel functions Jn**  
- **Sine & cosine eigenmodes in θ**  
- **Time-harmonic oscillations**

These represent vibrational modes of circular membranes (e.g., drums).  
Examples of computed modes (page 17):  
- u01, u02, u03  
- u11, u12, u13  
- u21, u22, u23  


---

### **🟦 2. Rectangular Membrane**  
Pages 9–13 show the full solution using:

- Double separation of variables  
- Fourier sine series in x and y  
- Two eigenvalue indices (n, m)  
- Mode shapes:

\[
u_{nm}(x,y,t) = (A_{nm}\cos \omega_{nm} t + B_{nm}\sin \omega_{nm} t)
\sin\left(\frac{n\pi x}{L}\right)\sin\left(\frac{m\pi y}{H}\right)
\]

Mode frequencies:  
\[
\omega_{nm} = c\sqrt{\left(\frac{n\pi}{L}\right)^2 + \left(\frac{m\pi}{H}\right)^2}
\]

Visual nodal patterns and 3D mode shapes (pages 14–16) show how each harmonic vibrates.  


---

## 🖥️ Numerical Results (FEATool Multiphysics)

### **Circular Membrane Modes**  
(Page 17)  
Includes colored 3D plots for multiple eigenmodes (u01, u02, u03 … u23), showing how vibration patterns propagate radially.

### **Rectangular Membrane Modes**  
(Pages 18–20)  
Modes such as:  
- (nx=1, ny=1)  
- (nx=1, ny=2)  
- (nx=2, ny=1)  
- (nx=2, ny=2)

These match the analytically derived mode structures.



---

## 🧩 Files in This Folder  
- **1105_Vibrating Membrane.pdf** — full analytical and numerical project report  
- **README.md** (this file)

---

## 📎 Conclusion  
The project demonstrates how membrane vibrations depend entirely on geometry, boundary conditions, and eigenvalues. Circular and rectangular geometries produce distinct eigenfunctions, and their vibrational modes can be predicted precisely using PDE theory. Numerical simulations validated the analytical forms, showing strong alignment with theoretical expectations.

This study highlights the fundamental role of PDEs in modeling real-world systems such as drums, biological membranes, sensors, and waveguides.

