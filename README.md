# 🌲🔥 Forest Fire Spread Visualizer

A web-based simulation tool that visualizes the spread of a wildfire through a forest grid. Built using a Python Flask backend and a React frontend, this project demonstrates how a fire spreads over time using **a Breadth-First Search (BFS) algorithm**. Users can draw a custom forest grid, simulate fire spread, and see how long it takes for the fire to burn all reachable trees.

---

## 🚀 Features

- Draw or generate a forest grid (empty land, healthy trees, and burned trees)
- Simulate daily fire spread based on adjacency
- Visualize which trees burn on each day
- See how many days it takes to burn all trees, or if some trees survive
- (Optional) Show graph of burned trees per day

---

## 🧠 Problem Description

Given a grid representing a forest where:
- `0` = empty land
- `1` = healthy tree
- `2` = burned tree

Each day, any healthy tree directly adjacent (up, down, left, right) to a burned tree will also catch fire. The simulation continues until either:
- All healthy trees are burned, or
- Some healthy trees cannot be reached by fire

The goal is to calculate:
- The number of days it takes to burn all healthy trees, or
- Return `-1` if some healthy trees cannot be reached

---

## 🧱 Tech Stack

| Layer     | Tool              | Purpose                       |
|-----------|-------------------|-------------------------------|
| Frontend  | React (Vite)      | Interactive UI + grid editor |
| Styling   | Tailwind CSS      | Fast, responsive styling      |
| Backend   | Flask (Python)    | Fire spread algorithm & API  |
| Logic     | BFS Algorithm     | Fire simulation engine        |
| Data Flow | Axios             | Send grid from React to Flask|

---

## 🛠️ How to Run It Locally

### 🔧 Backend (Flask)
1. Navigate to the `backend/` folder
2. Create a virtual environment:
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
3. Install dependencies:
   pip install flask flask-cors
4. Run the server:
   python app.py

💻 Frontend (React + Vite)
Navigate to the frontend/ folder
1. Install dependencies:
   npm install
2. Run the dev server:
   npm run dev

📈 Example Use Cases
Explore fire containment strategies

Visualize how fast fire spreads in different forest layouts

Demonstrate BFS algorithm in action

