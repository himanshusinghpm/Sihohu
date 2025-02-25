singapore-home-hunt/
├── README.md               # Project overview and quick start guide
├── requirements.txt        # Python dependencies
├── data/                   # Data storage
│   ├── properties.json     # Property listings data
│   ├── checkpoints.json    # Important locations
│   └── neighborhoods.json  # Area information
├── src/                    # Source code
│   ├── __init__.py         # Makes the directory a Python package
│   ├── data_manager.py     # Property data CRUD operations
│   ├── geo_utils.py        # Geospatial utilities
│   ├── map_visualizer.py   # Map visualization functions
│   ├── amenities.py        # Nearby amenities search
│   └── analysis.py         # Property comparison and scoring
├── notebooks/              # Jupyter notebooks
│   ├── 01_data_entry.ipynb      # Property data management
│   ├── 02_map_exploration.ipynb # Map visualization
│   └── 03_analysis.ipynb        # Property comparison
└── docs/                   # Documentation
    ├── modules/            # Module documentation
    ├── learning/           # Learning resources
    ├── decisions/          # Key decisions
    └── dictionary.md       # Data dictionary




# Sample Readme.md

## Singapore Home Hunt (SiHoHu)

A tool to track, visualize, and analyze potential homes in Singapore.

### Features
- Map-based property visualization
- Commute time analysis
- Nearby amenities search
- Property comparison and scoring

### Setup
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run Jupyter: `jupyter notebook`
4. Open the notebooks in the `notebooks/` directory



# Sample Markdown for Modules
## Map Visualizer Module

This module handles all map visualization functions.

## Key Functions

### visualize_properties(properties_list)
Displays all properties on an interactive map.

**Parameters:**
- `properties_list`: List of property dictionaries

**Returns:**
- A Folium map object

**Example:**
```python
map = visualize_properties(my_properties)
display(map)
```

# Sample Data Dictionary
## Data Dictionary

### Property Object

| Field         | Type       | Description                       | Example               |
|---------------|------------|-----------------------------------|-----------------------|
| id            | string     | Unique identifier                 | "prop_123"            |
| name          | string     | Property nickname/title           | "Sunny Orchard Condo" |
| address       | string     | Full address                      | "123 Orchard Rd"      |
| property_type | string     | HDB, Condo, or Landed             | "Condo"               |
| size_bhk      | integer    | Number of bedrooms                | 2                     |
| size_sqm      | float      | Size in square meters             | 85.5                  |
| price         | integer    | Price in SGD                      | 1200000               |
| rental        | integer    | Monthly rental in SGD (optional)  | 3500                  |
| location      | [lat, lng] | Coordinates                       | [1.3010, 103.8375]    |
| url           | string     | Link to listing                   | "https://example.com" |
| notes         | string     | Personal notes                    | "Great view, noisy"   |
| rating        | integer    | Personal rating (1-5)             | 4                     |
| viewed_on     | string     | Date viewed (YYYY-MM-DD)          | "2025-02-20"          |

# Sample Learning Resources File
## Python Geospatial Learning Resources

### Tutorials
- [Folium Tutorial](https://python-visualization.github.io/folium/quickstart.html)
- [GeoPandas Introduction](https://geopandas.org/en/stable/getting_started/introduction.html)

### Concepts Learned
- **2025-02-25**: Learned how to create basic maps with Folium
- **2025-02-26**: Implemented custom markers with popups

### Code Snippets
#### Creating a basic map centered on Singapore
```python
import folium
singapore_map = folium.Map(location=[1.3521, 103.8198], zoom_start=12)
singapore_map
```


# Sample Decision Log
## Decision Log

### 2025-02-25: Data Storage Format

**Decision**: Use JSON for data storage initially instead of CSV or a database.

**Rationale**:
- More flexible for nested data structures
- Easy to read and write with Python
- Simple to version control
- Doesn't require database setup

**Alternatives Considered**:
- CSV: Too flat for our data structure
- SQLite: More complexity than needed at this stage

**Future Considerations**:
- May migrate to SQLite or PostgreSQL if data volume increases


# AI Template
## Singapore Home Hunt Project Context

I'm building a tool to help me find housing in Singapore. The tool:
- Tracks properties I'm interested in
- Visualizes them on a map
- Analyzes commute times and nearby amenities
- Helps me compare options

My current focus is on: [specific module/feature]

Previous work: [brief summary or GitHub link]

My specific question: [clear, focused question]
