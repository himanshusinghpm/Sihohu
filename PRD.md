# Singapore Home Hunt (SiHoHu)
### Product Requirements Document

## 1. Introduction

### 1.1 Purpose
The Singapore Home Hunt (SiHoHu) tool is a personal application designed to streamline and enhance the process of finding suitable housing in Singapore. The tool will provide map-based visualization, data management, location analysis, and decision support for comparing housing options.

### 1.2 Target User
Initially, this product is designed for personal use to support house hunting in Singapore, with potential for expansion to benefit others relocating to Singapore or different cities.

### 1.3 Scope
The initial scope focuses on creating a data-driven tool for tracking and comparing housing options with particular emphasis on location analysis. The tool will be implemented as a Python application with interactive Jupyter notebooks.

## 2. Product Overview

### 2.1 Product Vision
SiHoHu will transform the overwhelming process of finding housing in an unfamiliar city into a structured, data-driven experience that enables confident decision-making based on personalized priorities.

### 2.2 Key Benefits
- Visual exploration of potential neighborhoods and properties
- Systematic tracking of housing options
- Objective comparison of properties based on customizable criteria
- Time savings through efficient location analysis
- Data-driven decision making

### 2.3 User Stories

**As a newcomer to Singapore, I want to:**
- View potential properties on a map to understand their location context
- Track details of properties I'm interested in from various listing websites
- Calculate commute times to important locations (office, airport, etc.)
- Find nearby amenities within walking distance
- Compare properties across multiple criteria to make informed decisions
- Remember areas I've explored and what I liked/disliked about them
- Document my house-hunting process for future reference

## 3. Feature Requirements

### 3.1 Map Exploration and Visualization

#### 3.1.1 Interactive Map
- **Must Have:** Interactive map of Singapore with property markers
- **Must Have:** Ability to add/edit/remove property markers
- **Must Have:** Different marker styles for different property types (HDB, condo, landed)

#### 3.1.2 Area Management
- **Must Have:** Save and label neighborhoods/areas of interest
- **Must Have:** Add personal landmarks and checkpoints (office, airport, etc.)
- **Should Have:** Draw boundaries around areas of interest

#### 3.1.3 Visual Distinctions
- **Must Have:** Color-coding of properties based on type
- **Must Have:** Visual indicators for property size (1BHK, 2BHK, etc.)
- **Should Have:** Heatmap visualization of personal ratings

### 3.2 Property Data Management

#### 3.2.1 Property Information
- **Must Have:** Store basic property details (address, price, size, type)
- **Must Have:** Record geographic coordinates for mapping
- **Must Have:** Add personal notes and impressions
- **Should Have:** Store photos or links to virtual tours
- **Should Have:** Track viewing appointments and status updates

#### 3.2.2 Data Operations
- **Must Have:** Add new properties (manually entered)
- **Must Have:** Edit existing property information
- **Must Have:** Remove properties no longer of interest
- **Must Have:** Export/backup property data
- **Should Have:** Bulk import capabilities

### 3.3 Location Analysis

#### 3.3.1 Commute Analysis
- **Must Have:** Calculate distances to important places
- **Must Have:** Estimate commute times for different transportation modes
- **Should Have:** Visualize commute routes on the map
- **Could Have:** Time-based analysis (peak hour vs. off-peak)

#### 3.3.2 Amenities Search
- **Must Have:** Find nearby amenities (groceries, MRT stations, bus stops)
- **Must Have:** Calculate walking distances to key amenities
- **Should Have:** Filter amenities by type
- **Should Have:** Set custom search radius

#### 3.3.3 Neighborhood Assessment
- **Should Have:** Track neighborhood characteristics
- **Could Have:** Access to neighborhood safety data
- **Could Have:** Flood risk or environmental factors

### 3.4 Decision Support

#### 3.4.1 Property Comparison
- **Must Have:** Side-by-side comparison of properties
- **Must Have:** Customizable scoring system
- **Should Have:** Visualization of tradeoffs between options

#### 3.4.2 Personalization
- **Must Have:** Apply personal weights to different criteria
- **Must Have:** Define must-have vs nice-to-have features
- **Should Have:** Preset comparison templates for different priorities

#### 3.4.3 Decision Documentation
- **Should Have:** Record decision rationale
- **Should Have:** Track eliminated options and reasons

## 4. Technical Requirements

### 4.1 Technology Stack
- Python 3.8+ as the core programming language
- Jupyter Notebook for interactive development and visualization
- Pandas for data manipulation
- Folium/Plotly for interactive maps and visualizations
- GeoPy for geospatial calculations
- JSON for data storage (initially)

### 4.2 System Requirements
- **Platform:** Desktop/laptop with modern web browser
- **Dependencies:** Python environment with required packages
- **Performance:** Responsive map rendering with up to 100 property markers

### 4.3 Development Requirements
- Modular code structure for maintainability
- Comprehensive documentation for learning purposes
- Version control via GitHub
- Step-by-step learning approach

## 5. Constraints and Limitations

### 5.1 Technical Constraints
- Initially using static data files rather than a database
- Limited to publicly available APIs for location data
- No real-time property listing integration (manual data entry)

### 5.2 Timeline Constraints
- Development will progress alongside the actual house-hunting process
- Features prioritized based on immediate needs

## 6. Development Phases

### 6.1 Phase 1: Foundation (Week 1-2)
- Project setup and repository creation
- Design data model for properties and checkpoints
- Implement basic data management functionality
- Create simple map visualization

### 6.2 Phase 2: Core Features (Week 3-4)
- Add property markers with detailed information
- Implement checkpoint creation and display
- Calculate basic distances and commute times
- Create basic property comparison functionality

### 6.3 Phase 3: Advanced Features (Week 5-6)
- Integrate with transportation APIs for better commute estimates
- Add nearby amenities search
- Implement custom scoring system
- Create detailed property comparison views

### 6.4 Phase 4: Refinement (Week 7-8)
- Enhance visualization with additional layers
- Add advanced filtering and search
- Improve user experience in notebooks
- Add data export and reporting

## 7. Success Metrics

### 7.1 Personal Usage Metrics
- Successfully track at least 20 potential properties
- Reduce time spent researching locations by 50%
- Gain comprehensive understanding of 5+ Singapore neighborhoods
- Make a confident, data-informed housing decision

### 7.2 Technical Success Metrics
- Create a reusable codebase for future city relocations
- Learn and apply Python geospatial libraries
- Document the development process for learning purposes

## 8. Appendices

### 8.1 Data Schema

#### Property Object (Draft)
```json
{
  "id": "prop_123",
  "name": "Sunny Orchard Condo",
  "address": "123 Orchard Rd",
  "property_type": "Condo",
  "size_bhk": 2,
  "size_sqm": 85.5,
  "price": 1200000,
  "rental": 3500,
  "location": [1.3010, 103.8375],
  "url": "https://example.com/listing",
  "notes": "Great view, noisy area",
  "rating": 4,
  "viewed_on": "2025-02-20"
}
```

#### Checkpoint Object (Draft)
```json
{
  "id": "cp_office",
  "name": "Office",
  "type": "work",
  "location": [1.2966, 103.8500],
  "importance": "high",
  "notes": "Main workplace"
}
```

### 8.2 Third-Party Resources
- OneMap Singapore API
- OpenStreetMap
- Land Transport Authority (LTA) DataMall
- Urban Redevelopment Authority (URA) Space
