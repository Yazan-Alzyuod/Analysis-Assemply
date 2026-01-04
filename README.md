# Analysis-Assemply
# 🏗️ ANSYS Static Structural Analysis of Mechanical Assembly

## 📋 Project Overview
This repository contains a **static structural analysis** of a mechanical assembly consisting of multiple interconnected parts, performed in **ANSYS Mechanical**. The simulation evaluates deformation, stress distribution, and safety factors under pressure loading, demonstrating assembly-level finite element analysis.

---

## 🎯 Key Results

### 📏 **Maximum Total Deformation:** 0.9077 µm
![Assembly Deformation](Assemply.jpg)

### ⚠️ **Maximum Equivalent Stress:** 3.654 MPa
### 🔒 **Safety Factor:** >15 (Minimum)

---

## 🏗️ **Assembly Specifications**

### 📐 **Geometry & Assembly**
- **Source:** Imported from IGES file (`Assem1.IGS`)
- **Total Dimensions:** 100mm (X) × 60mm (Y) × 150mm (Z)
- **Assembly Volume:** 2.5652e-004 m³ (256.52 cm³)
- **Total Mass:** 2.0137 kg
- **Number of Bodies:** 4 (2 unique parts, each appearing twice)
- **Parts Configuration:** Symmetrical assembly

### 🔩 **Part Details**

| Part | Quantity | Dimensions (X×Y×Z) | Volume (m³) | Mass (kg) | Material |
|------|----------|-------------------|-------------|-----------|----------|
| **Part1[Solid]** | 2 | 100mm × 60mm × 20mm | 1.1655e-004 | 0.91494 | Structural Steel |
| **Part2[Solid]** | 2 | 13.817mm × 13.817mm × 150mm | 1.1705e-005 | 0.091888 | Structural Steel 2/3 |

### 🔗 **Contact Definitions**
- **Total Contacts:** 4 bonded contact regions
- **Contact Type:** Bonded (perfect connection)
- **Detection Method:** Automatic face pairing
- **Tolerance:** 0.475 mm (automatic detection)

### ⚙️ **Material Properties** (All Structural Steel Variants)
| Property | Value | Unit |
|----------|-------|------|
| Density | 7850 | kg/m³ |
| Young's Modulus | 200 | GPa |
| Poisson's Ratio | 0.3 | - |
| Yield Strength | 250 | MPa |
| Ultimate Tensile Strength | 460 | MPa |
| Thermal Expansion Coefficient | 1.2 × 10⁻⁵ | 1/°C |

*Note: Structural Steel, Structural Steel 2, and Structural Steel 3 have identical properties in this analysis.*

---

## 🔧 **Boundary Conditions & Loading**

### 🏗️ **Constraints**
- **Fixed Support 1:** Face constraint on Part1
- **Fixed Support 2:** Face constraint on Part1 (opposite side)
- **Constraint Type:** Fully fixed (all degrees of freedom)

### ⬇️ **Applied Load**
- **Load Type:** Uniform Pressure
- **Magnitude:** 3.0 MPa
- **Application:** Normal to selected surface
- **Load Distribution:** Uniform across face

### ⚙️ **Solver Settings**
- **Analysis Type:** Static Structural
- **Solver:** Mechanical APDL
- **Time Step:** 1 second
- **Large Deflection:** Off
- **Contact Formulation:** Program Controlled
- **Solution Method:** Direct sparse matrix solver

---

## 📈 **Analysis Results Summary**

### 🎯 **Deformation Analysis**
- **Maximum Total Deformation:** 9.0873e-7 m (0.9077 µm)
- **Average Deformation:** 2.8555e-7 m (0.2856 µm)
- **Deformation Pattern:** Symmetrical distribution
- **Location of Maximum:** Part1[Solid] components

### ⚠️ **Stress Analysis**
- **Maximum Equivalent (von-Mises) Stress:** 3.6541 MPa
- **Minimum Equivalent Stress:** 1.3708 kPa
- **Average Equivalent Stress:** 0.60506 MPa
- **Critical Locations:** Contact regions and constrained areas
- **Stress Concentration:** Minimal, well-distributed

### 🔒 **Safety Analysis**
- **Minimum Safety Factor:** >10 (actual: 15)
- **Maximum Safety Factor:** 15
- **Average Safety Factor:** 15
- **Safety Criterion:** Maximum Equivalent Stress / Yield Strength
- **Margin of Safety:** Significant (stress levels far below yield)

### 📊 **Mesh Quality**
- **Total Nodes:** 5,296
- **Total Elements:** 1,960
- **Element Type:** 3D Solid Elements
- **Mesh Quality:** Program controlled, medium smoothing
- **Convergence:** Achieved with Newton-Raphson method
## 👨‍💻 Author
**Yazan Alzyuod**
* **Mechanical Engineer**
* 📧 [yqlasem@gmail.com](mailto:yqlasem@gmail.com)
* 🔗 [LinkedIn Profile](https://www.linkedin.com/in/yazan-alzyuod  )
* 💻 [GitHub Profile](https://github.com/Yazan-Alzyuod  )
* 📞 00962775327776   use this for information in the end
