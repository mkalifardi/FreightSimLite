# FreightSimLite

**FreightSimLite** is an open-source, Python-based simulation tool designed to model and visualize freight delivery agent behavior in urban road networks using real GIS data. It focuses on last-mile logistics and urban freight analysis, suitable for academic research and city planning.

## Features

- Import real road networks from OpenStreetMap using `osmnx`
- Define custom delivery agents and depot points
- Compute shortest paths with congestion-neutral logic
- Visualize delivery routes over the actual road network
- Export delivery trip logs for analysis

## Requirements

- Python 3.8+
- osmnx
- networkx
- pandas
- matplotlib

Install all dependencies:
```bash
pip install -r requirements.txt
```

## Folder Structure

```
freightsimlite/
│
├── data/                   # Raw GIS data or delivery input files
├── outputs/                # Simulation results and trip logs
├── scenarios/              # (Optional) Scenario configurations
├── notebooks/              # Interactive analysis or visualizations
├── freightsimlite.py       # Main simulation script
├── README.md               # Project overview (you are here)
├── requirements.txt        # Python dependencies
└── LICENSE                 # Open-source license
```

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/yourusername/freightsimlite.git
cd freightsimlite
```

2. Run the simulation:
```bash
python freightsimlite.py
```

This will:
- Generate 10 synthetic freight agents
- Assign delivery locations randomly in Melbourne
- Visualize their delivery paths
- Export a CSV log in `outputs/trip_log.csv`

## Output
- **Visual map** with delivery routes plotted
- **CSV file** of trip logs:
  - `agent_id`, `origin_node`, `destination_node`, `departure_time`

## Use Cases
- Freight policy scenario testing (e.g., toll roads, restricted zones)
- Last-mile delivery research
- Urban logistics education tools

## License
MIT License — free to use, modify, and distribute.

---

### Inspired by goals in:
- Freight simulation
- Multi-agent modeling
- Transport engineering research

Want to contribute? Open an issue or fork the project!
