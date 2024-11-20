# Pedestrian-Friendly Areas in Cologne: SVM Analysis
## Overview
This project uses Support Vector Machines (SVM) to classify pedestrian-friendly areas in Cologne, Germany, based on real-world data fetched from OpenStreetMap (OSM). The analysis incorporates pedestrian, traffic, and cycleway routes and visualizes the decision boundary, feature importance, and routes on a map.

## Table of Contents
1. Overview
2. Data Sources
3. Features
4. Installation
5. Usage
6. Visualizations
7. Results
8. Contributing
9. License

## Data Sources
The data for this project is fetched directly from OpenStreetMap using the osmnx library. Key data includes:
- Pedestrian routes (highway=footway, highway=pedestrian, highway=path)
- Traffic roads (highway=motorway, highway=primary, highway=secondary, highway=tertiary)
- Cycleways (highway=cycleway)
- 
## Features
1. Fetch Data from OpenStreetMap: Retrieves all pedestrian routes, traffic roads, and cycleways for Cologne.
2. Simulated Neighborhood Data: Generates 100 data points with realistic variations for training.
3. SVM Model: Trains a linear SVM model on the scaled dataset.
4. Visualization: Visualizes the SVM decision boundary, maps routes, and displays feature importance.
   
## Installation
### Step 1: Clone the Repository
///bash
git clone https://github.com/your-username/pedestrian-friendly-cologne.git
cd pedestrian-friendly-cologne
///
### Step 2: Install Dependencies
///bash
pip install -r requirements.txt
///

## Usage
Run the script to generate the visualizations and results:
///bash
python pedestrian_analysis.py
///

The script fetches data from OpenStreetMap, simulates neighborhood data, trains an SVM model, and generates visualizations.

## Visualizations
This project generates the following visualizations:
1. SVM Decision Boundary: Displays the classification of pedestrian-friendly areas.
2. Confusion Matrix: Evaluates the model's performance.
3. Feature Importance Plot: Highlights the most influential features in the SVM model.
4. Pedestrian Routes Map: Visualizes pedestrian, traffic, and cycleway routes in Cologne.

## Results
The SVM model provides the following outputs:
- Classification Accuracy: Evaluated using a confusion matrix.
- Feature Importance: Determines which features most impact the pedestrian-friendly classification.
- Visual Map: Displays Cologne's pedestrian routes alongside traffic and cycleways.

## Contributing
Contributions are welcome! If you have ideas for improvement or find any issues, feel free to:
1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Submit a pull request.
   
## License
This project is licensed under the MIT License.
