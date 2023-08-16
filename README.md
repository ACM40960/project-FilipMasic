[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/foXtNvtG)



# Identification and Ranking of Optimal Locations for New Electric Vehicle (EV) Charging Stations in Dublin

## Motivation

We're tackling the challenge of identifying the best spots for new EV charging stations in Dublin, contributing to the city's eco-friendly and clean mobility goals.

## Why It Matters

As the world shifts towards greener transportation options, EVs have gained prominence for their reduced emissions and environmental benefits. To support this transition, we're working on creating an optimal network of EV charging stations in Dublin, ensuring easy access for EV owners. 

## How It Works

Our approach involves data-driven decision-making and optimization algorithms while obtaining data from readily available sources:

### 1. Data Collection and Exploration: 
   - To get started, we need data! Gather diverse datasets that include:
   - Existing charging station locations
   - Demographic factors
   - Traffic density
   - Proximity to amenities
   - Other features influencing charging station demand and usage patterns.

### 2. Data Processing and Feature Engineering:
   - Clean and pre-process the collected data.
   -  Calculate metrics like:
      - Proximity to existing charging stations
      - Distance to public service spots
      - Pobal's deprivation index
      - Population density, etc.

### 3. Objective (Weight) Function Formulation: 
   - Formulate an objective (weight) function that considers the various features. This function guides the optimization process to select the most suitable locations for new EV charging stations.

### 4. Optimization Algorithms:
   - We employ algorithms like Mixed-Integer Linear Programming (MILP) and ranking functions to pinpoint the optimal charging station locations.

### 5. Results and Recommendations:
   - Based on optimization results, we identify the top spots for new EV charging stations in Dublin. This information aids policymakers, urban planners, and stakeholders in strategically deploying charging infrastructure.

## Getting Started


- Install required Python packages:
- Prepare your data:
   - Create a data directory and place your CSV files inside.
   -Ensure your hotspot.csv contains potential charging station locations and features.csv lists nearby amenities.

    Open the ev_charging_optimization.ipynb notebook in Jupyter Notebook or Jupyter Lab. This is where the magic happens!

## Data Format

To ensure compatibility, your hotspot.csv and features.csv files should follow these formats:

### hotspot.csv:

    Columns: location_id, latitude, longitude
    Each row represents a potential charging station location.
    Example:

    python

    location_id,latitude,longitude
    1,53.349805,-6.26031
    2,53.363186,-6.241974
    ...

### features.csv:

    Columns: location_id, amenity, distance_to_station
    Each row represents an amenity near a potential charging station.
    Example:

    python

    location_id,amenity,distance_to_station
    1,Public Service,500
    1,Café,300
    2,Park,700
    ...

## Contact Us

For any questions or feedback, reach out to Your Name.

## License

This project is licensed under the MIT License.

We're excited to have you on board to contribute to the transformation of Dublin's transportation landscape towards a greener and more sustainable future. Let's work together to make a positive impact!

