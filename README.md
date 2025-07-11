# Malawi Districts Graph Layout Optimization

This project optimizes the visual layout of a graph representing Malawi’s 28 districts and their inter-district connections using a force-directed layout algorithm (`d3-force`). The final node positions are normalized within a 1x1 unit square to ensure a clean, readable graph.

---

## 📌 Objective

Given initial coordinates and district connections:
- Improve node distribution to reduce clutter and overlaps.
- Make connected districts appear closer together.
- Keep all node positions inside a 1x1 bounding box.

---

## ⚙️ Tech Stack

- Node.js
- JavaScript
- [`d3-force`](https://github.com/d3/d3-force)

---

## 🧠 Algorithm Used

**Force-Directed Layout** using `d3-force`:
- Nodes are repelled from each other (forceManyBody).
- Connected nodes are pulled together (forceLink).
- Node positions are kept within bounds (normalized).
- A collision force is applied to prevent overlaps.

---

## 🚀 How to Run

### 1. Clone and install
```bash
git clone https://github.com/your-username/malawi-layout.git
cd malawi-layout
npm install
