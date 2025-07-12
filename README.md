# 🇲🇼 Malawi Districts Graph Layout Optimization

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
- [`d3-array`](https://github.com/d3/d3-array) (for normalization)

---

## 🧠 Algorithm Used

**Force-Directed Layout** using `d3-force`:
- `forceManyBody` to repel nodes from each other.
- `forceLink` to pull connected districts closer together.
- `forceCenter` to keep layout centered in view.
- `forceCollide` to prevent node overlaps.
- Normalized output using `d3-array.extent()`.

---

## 🚀 How to Run

### 1. Clone and install dependencies
```bash
git clone https://github.com/maulidiphilip/malawi-layout.git
cd malawi-layout
npm install
````

### 2. Run the layout simulation

```bash
node layout.js
```

✔️ This generates `optimized_nodes.json` containing final coordinates inside `[0, 1]`.

---

## 🌐 Visualize the Graph

Open `index.html` in any modern browser to:

* View interactive layout
* Hover on districts for names
* Drag nodes to explore layout

---

## 📂 Files

```
malawi-layout/
├── layout.js                # Node simulation script
├── optimized_nodes.json     # Final coordinates after layout
├── index.html               # Visualization using D3
├── package.json             # Dependency config
├── screenshots/layout.png   # Screenshot for submission
├── README.md               
```

---

