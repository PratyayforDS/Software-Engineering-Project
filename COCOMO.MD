#  COCOMO-Based Effort and Schedule Estimation for a Medium-Complexity Project

This document provides a **Basic COCOMO** (Constructive Cost Model) estimation for the effort, schedule, and implied team size required for the software development project.

---

##  Model Selection and Rationale

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Model Used** | Basic COCOMO | The simplest version, suitable for a quick, initial estimation. |
| **Mode Used** | Semi-Detached | This mode is appropriate for projects of **medium size and complexity**, characterized by:<ul><li>A small, mixed-experience development team.</li><li>Integration of existing components (e.g., OCR engine, LLM APIs, web frontend).</li></ul> |
| **Assumed Project Size (KLOC)** | 2.7 | Estimated from current prototype size (~600 LOC), applying realistic expansion factor (4–5× growth) |

---

##  COCOMO Parameters (Semi-Detached Mode)

The following parameters are used in the estimation formulas for the **Semi-Detached** mode:

$$E = a \times (\text{KLOC})^b$$
$$T = c \times (E)^d$$

| Parameter | Value |
| :--- | :--- |
| $a$ | 3.0 |
| $b$ | 1.12 |
| $c$ | 2.5 |
| $d$ | 0.35 |

---

##  Effort Estimation (E)

The **Effort ($E$)** is the total person-months required to complete the project.

**Formula:** $E = a \times (\text{KLOC})^b$

**Calculation:**
$$E = 3.0 \times (2.7)^{1.12}$$
$$E \approx 3.0 \times 3.03$$
$$E \approx 9.09 \text{ person-months}$$

**Estimated Effort:** $\mathbf{\approx 9.1 \text{ person-months}}$

---

##  Schedule Estimation (T)

The **Development Time ($T$)** is the total calendar months required for the project.

**Formula:** $T = c \times (E)^d$

**Calculation:**
$$T = 2.5 \times (9.09)^{0.35}$$
$$T \approx 2.5 \times 2.15$$
$$T \approx 5.38 \text{ months}$$

**Estimated Development Time:** $\mathbf{\approx 5.4 \text{ months}}$

---

### **Summary of Key Results**

| Metric | Estimated Value |
| :--- | :--- |
| **Total Effort (E)** | $\mathbf{9.1 \text{ person-months}}$ |
| **Development Time (T)** | $\mathbf{5.4 \text{ months}}$ |