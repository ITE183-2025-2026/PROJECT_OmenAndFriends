# PROJECT_OmenAndFriends  
## Deployment Simulation Program  

---

### 📖 Overview
This project is a **Deployment Assignment Simulation** built with a frontend mapping interface and backend assignment logic.  
It allows users to place patrol markers on a map, assign them dynamically or manually, and visualize coverage areas, adjacency polylines, and strategy outcomes.  

![Untitled design](https://github.com/user-attachments/assets/6e56c7f2-582a-4b9a-b162-6c17e6c078df)

**Key Features:**
- **Marker placement** with NATO naming order.
- **Strategy selection**: Maximal (independent sets) or Maximum (maximize assignments).
- **Overrides**: Adjust max assigned markers and strategy radius.
- **Auto-assign toggle**: Runs every 2 seconds of user inactivity, enforcing overlap rules.
- **Manual controls**: Popups for renaming, radius adjustment, and assignment toggling.
- **Sidebar sync**: Reflects assigned vs idle markers.
- **Utility actions**: Unassign all patrols, clear all markers.

---

### 🎯 Scope
The Deployment Simulation Program is designed as a **prototype and teaching tool** for exploring patrol assignment strategies.  

**It focuses on:**
- Demonstrating **assignment algorithms** (independent set vs maximum assignment).  
- Visualizing **marker coverage, overlaps, and adjacency** with polylines and radius circles.  
- Allowing **user interaction** through manual overrides and auto‑assign toggles.  
- Providing a **sandbox environment** for experimenting with patrol distribution logic.  

**Out of scope:**
- Real‑world deployment or integration with live patrol systems.  
- Persistent storage of assignments (data resets on refresh).  
- Advanced GIS features beyond basic map rendering and heatmap overlays.  

---

### ⚙️ How to Install
1. Clone the repository:
   ```bash
   git clone https://github.com/ChanPagar/PROJECT_OmenAndFriends.git
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the development server:
   ```bash
   npm run dev
   ```

**Demo:**  
Launch the app in your browser (default: http://localhost:5173 or http://localhost:3000 depending on your setup).

Place markers on the map. They will be named in NATO order (Alpha, Bravo, Charlie…).

Open the Action Panel to:
- Switch between **Maximal** and **Maximum** strategies.
- Adjust maximum assigned markers or strategy radius.
- Toggle **Auto-assign** (debounced every 2s of inactivity).
- Use **Unassign All** or **Clear All** buttons.

**Observe:**
- Sidebar updates with assigned/idle markers.
- Popups show marker details, allow renaming, and radius adjustment.
- Backend logic enforces overlap rules and heatmap priorities.

---

### 🛠️ Technologies Used
- **FastAPI (Python)** – backend orchestration and assignment logic  
- **React.js** – frontend interface and component management  
- **Vanilla JavaScript (with jQuery)** – UI utilities, circle progress, and DOM interactions  
- **Svelte Range Slider Pips** – interactive slider for patrol assignment limits  
- **Leaflet.js** – map rendering, drawing tools, and heatmap visualization  
- **CSS (modularized)** – styling for panels, toggles, sliders, and map UI  

---

### 👥 Proponents
- **Leader:** Christian Joey Pagar  
- **Members:**  
  - Wilson Augosto  
  - Jerrold Canoneo  

---

### 📊 Block Diagram
<img width="1081" height="1496" alt="flowchart_thesis drawio" src="https://github.com/user-attachments/assets/de96ed19-e415-49ed-a3fc-3c067059b573" />

