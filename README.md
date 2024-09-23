

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
### 1. Optimized Route Map
This map visualizes the optimized delivery route, highlighting customer locations along the path. Each customer is marked with a number indicating the sequence of visits, and the route is illustrated with arrows.


<img width="938" alt="Screenshot 1446-03-20 at 3 09 05 AM" src="https://github.com/user-attachments/assets/c0787a79-df57-40e4-b825-69a5706031b9">

*The green marker indicates the starting point, while the red marker represents the endpoint. The blue lines show the optimized route connecting the customers.*

### 2. Bar Chart of Total Pallets Assigned per Truck

![Unknown-25](https://github.com/user-attachments/assets/f79ccfeb-95fe-4955-bf35-e9f86243b31f)
*This bar chart illustrates the total number of pallets assigned to each truck, highlighting the workload distribution.*

## Requirements
- Python 3.x
- Pandas
- Folium
- Matplotlib
- Seaborn
- OR-Tools

