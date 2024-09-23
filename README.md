# Logistics Optimization Project

## Overview
This project implements a logistics optimization solution for truck assignments and route planning based on customer orders. It leverages data from sales orders, customer locations, and truck capacities to optimize delivery routes and visualize the results.

## Features
- **Data Aggregation**: Computes total pallets per customer based on sales orders.
- **Truck Assignment**: Assigns customers to trucks based on their pallet requirements and truck capacities.
- **Route Optimization**: Utilizes distance calculations to determine the most efficient delivery routes.
- **Data Visualization**: Creates interactive heatmaps and bar charts to visualize customer distribution and truck assignments.

## Code Functionality
1. **Data Loading**: The code loads necessary datasets from CSV files, including orders, customers, trucks, and products.
2. **Pallet Calculation**: Computes the number of pallets required for each customer based on their orders.
3. **Customer and Truck Data Merging**: Merges customer data with the aggregated pallet information to facilitate assignments.
4. **Truck Assignment Logic**: Assigns trucks to customers while ensuring that each truck's capacity is not exceeded.
5. **Distance Matrix Creation**: Computes the distance between customer locations for route optimization.
6. **Route Optimization**: Uses Google OR-Tools to determine the optimal delivery routes.
7. **Visualization**: Generates a geographical heatmap to visualize customer density and a bar chart to show the total pallets assigned to each truck.

## Outputs
### 1. Geographical Heatmap
![Geographical Heatmap](path/to/heatmap_image.png)
*This heatmap shows the distribution of customer locations based on density.*

### 2. Bar Chart of Total Pallets Assigned per Truck
![Bar Chart](path/to/bar_chart_image.png)
*This bar chart illustrates the total number of pallets assigned to each truck, highlighting the workload distribution.*

## Requirements
- Python 3.x
- Pandas
- Folium
- Matplotlib
- Seaborn
- OR-Tools

## Installation
To install the required packages, you can use the following pip command:
```bash
pip install pandas folium matplotlib seaborn ortools
