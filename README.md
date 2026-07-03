# ⚙️ 4-Bar Synthesizer: Differential Evolution Solver

A high-performance computation engine designed to solve complex 4-bar linkage synthesis problems using a custom **Differential Evolution (DE)** algorithm.

---

## 📸 Interface Preview
![Project Web Interface](<img width="1826" height="853" alt="image" src="https://github.com/user-attachments/assets/4cad1495-df9d-4e40-984d-c56856114a9d" />
)

## 🌐 Live Demo
You can view the rendered interface of this synthesizer here:
**[View Interactive Web Interface](http://htmlpreview.github.io/?https://github.com/devyanids/4-Bar-Synthesizer/blob/main/4%20Bar%20Mechanism%20Synthesizer.html)**

---

## 🚀 SDE Engineering Highlights

* **Algorithmic Optimization:** Developed a custom Differential Evolution solver to optimize 8-dimensional coordinate arrays, systematically scoring candidates using a specialized loss function based on Euclidean distance and physical boundary checks.
* **Asynchronous Processing:** Offloaded heavy mathematical evaluation loops (800,000+ iterations) onto asynchronous background workers. This critical architectural decision prevented UI freezing and maintained a stable **60 FPS** interactive canvas.
* **Data Handling:** Implemented efficient data parsers to convert raw, high-throughput memory arrays into structured, analysis-ready CSV formats.

---

## 🛠️ Tech Stack

* **Core:** Python 3.8+
* **Concurrency:** `asyncio`, `threading`
* **Numerical Computing:** `NumPy`
* **Data Processing:** `Pandas`

---

## 📁 Repository Structure

```text
4-Bar-Synthesizer/
│
├── image_4930c0.png        # Project interface preview
├── src/                    # Optimization engine and background workers
├── data/                   # Processed coordinate arrays
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation
