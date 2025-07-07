# 🚗 Dynamic Parking Pricing Simulator

This project simulates real-time dynamic parking pricing using vehicle data, congestion levels, and geospatial analysis. It aims to optimize pricing based on demand, competition, and environmental conditions.

---

## 🧰 Tech Stack

- Python
- Pandas & NumPy
- Bokeh (for visualization)
- Geopy (for Haversine distance)
- Jupyter/Colab-compatible

---

## 📌 Key Features

- Demand-based pricing model
- Competitor-aware pricing adjustment
- Real-time visualization using Bokeh
- Clean feature encoding and timestamp handling

---

## 🏗️ Architecture Diagram

Check out [`architecture.md`](architecture.md) or the diagram in `architecture.png`.

---

## 🚀 How to Run

1. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2. Run the simulation:
    ```bash
    python simulation.py
    ```

3. Output: A Bokeh interactive plot showing parking price evolution.

---

## 🧠 How It Works

1. Load dataset and combine date+time into a timestamp
2. Generate Lot IDs from lat/long locations
3. Compute:
   - Occupancy Rate
   - Vehicle weight factor
   - Demand score (based on traffic, queues, holidays, vehicle type)
4. Adjust pricing based on:
   - Demand score
   - Competition (Haversine distance to other lots)
5. Smooth transition for price stability
6. Visualize real-time price changes with Bokeh

---

## 📃 License

Open-source project under the [MIT License](LICENSE).

---

## 📂 Project Structure

```bash
dynamic-parking-pricing/
├── simulation.py # Main simulation script
├── data/dataset.csv # Real-world dataset used for simulation
├── diagrams/ # Architecture or flow diagrams
├── README.md # This file
├── requirements.txt # Python dependencies
└── architecture.md # Architecture explanation (or image)
