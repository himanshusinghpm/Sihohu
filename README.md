# Singapore Home Hunt (SiHoHu)

A personal tool to streamline house hunting in Singapore by visualizing, analyzing, and comparing potential homes on a map.


## 🏠 Overview

Finding the perfect home in a new city like Singapore involves balancing many factors - location, commute times, amenities, and more. This tool helps me:

- Track properties I'm interested in from various listing websites
- Visualize them on a map to understand neighborhoods better
- Analyze commute times to important places (office, airport, etc.)
- Find nearby amenities (groceries, MRT stations, gyms, schools)
- Compare properties using customizable criteria
- Make data-driven decisions about where to live

## 🔍 Features

### Map Exploration
- Interactive map of Singapore with property markers
- Color-coded visualization based on property type and size
- Save and annotate neighborhoods and areas of interest
- Add personal landmarks and checkpoints

### Property Management
- Store detailed information about properties
- Save photos, links, and agent contacts
- Record personal impressions from viewings
- Track application status

### Location Analysis
- Calculate commute times to important places
- Find nearby amenities within walking distance
- Analyze neighborhood characteristics
- Compare air quality, flooding risks, etc.

### Decision Support
- Custom scoring system based on personal preferences
- Side-by-side property comparison
- Visualization of tradeoffs
- Documentation of decision-making process

## 🛠️ Technology Stack

- **Python**: Core programming language
- **Jupyter Notebooks**: Interactive development and visualization
- **Pandas**: Data manipulation and analysis
- **Folium/Plotly**: Interactive maps and visualizations
- **GeoPy**: Geospatial calculations
- **OpenStreetMap/OneMap API**: Location data and routing

## 🔄 Project Status

This project is in active development as I search for housing in Singapore. See [STATUS.md](docs/STATUS.md) for current progress.

## 📂 Repository Structure

```
singapore-home-hunt/
├── README.md               # Project overview
├── requirements.txt        # Python dependencies
├── data/                   # Data storage
│   ├── properties.json     # Property listings
│   └── checkpoints.json    # Important locations
├── src/                    # Source code
│   ├── data_manager.py     # Data operations
│   ├── geo_utils.py        # Geospatial utilities
│   ├── map_visualizer.py   # Map visualization
│   ├── amenities.py        # Nearby amenities search
│   └── analysis.py         # Property comparison
├── notebooks/              # Jupyter notebooks
│   ├── 01_data_entry.ipynb
│   ├── 02_map_exploration.ipynb
│   └── 03_analysis.ipynb
└── docs/                   # Documentation
    ├── modules/            # Module documentation
    ├── learning/           # Learning resources
    ├── decisions/          # Key decisions
    └── dictionary.md       # Data dictionary
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Git
- Jupyter Notebook/Lab

### Setup
1. Clone this repository
   ```bash
   git clone https://github.com/yourusername/singapore-home-hunt.git
   cd singapore-home-hunt
   ```

2. Create a virtual environment
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter
   ```bash
   jupyter notebook
   ```

5. Open the notebooks in the `notebooks/` directory to begin

## 📝 Learning Journey

This project also serves as a practical way to learn:
- Python programming
- Data management and storage
- Geospatial analysis
- Interactive visualization
- API integration

See the [learning log](docs/learning/log.md) for my ongoing notes.

## 🔮 Future Plans

- Add machine learning to predict property prices
- Integrate with property listing APIs if available
- Create a simple web interface for easier interaction
- Add historical price trends for neighborhoods

## 📚 Resources

- [OneMap Singapore API](https://www.onemap.gov.sg/docs/)
- [Folium Documentation](https://python-visualization.github.io/folium/)
- [Land Transport Authority DataMall](https://datamall.lta.gov.sg/content/datamall/en.html)
- [URA Space](https://www.ura.gov.sg/maps/)
