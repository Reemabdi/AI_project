# AI-Driven Pathfinding with A* Algorithm#

## Overview
This project implements the A* (A-star) algorithm to identify the most efficient path for a robot navigating a 100x100 grid, avoiding obstacles. The approach ensures optimal performance in terms of time and distance while accommodating barriers. The robot's movement is restricted to adjacent cells in eight possible directions.

Features
Algorithm: A* algorithm with customizable heuristics.
Grid-Based Simulation: Handles pathfinding on a 100x100 grid with variable obstacle densities.
Realistic Constraints: Incorporates movement restrictions and dynamic environments.
Performance Analysis: Evaluates success rates, path costs, and computational time across different obstacle densities.

# Installation
Install newest version of [python](https://www.python.org/) 

Run the algorithm:
python astar.py


## Problem Formulation Initial State:
**Start node**  (x, y, 0, 0), where x and y are integers in the range [0, 99].

**Goal State:** End node (x, y, 0, 0), where x and y are integers in the range [0, 99]. 

**State Space:** All nodes in a 100x100 grid.

**Goal Test:** Determines whether the current state is the goal state. 

**Actions:** The robot can move in eight directions: up, down, left, right, up-left, up-right, down-left, down-right. Implementation of A* Algorithm 


### Results Analysis
The algorithm's performance was evaluated in terms of pathfinding success rate, path cost, and computational time. 

### Summary of Results
•	Obstacle Density of 10%: 


Path Found: 100% success rate

Path Cost: Relatively low and consistent 

Average Time: Efficient 

•	Obstacle Density of 20%: 


Path Found: 100% success rate

Path Cost: Increased variability

Average Time: Slightly increased

•	Obstacle Density of 30%: 


Path Found: 95% success rate 

Path Cost: More variability and higher costs

Average Time: Noticeably higher

•	Obstacle Density of 40%: 


Path Found: 80% success rate 

Path Cost: Higher and more variable

Average Time: Significantly higher


•	Obstacle Density of 50%: 

Path Found: 55% success rate

Path Cost: High variability and cost 

Average Time: High 


•	Obstacle Density of 60%:

Path Found: 15% success rate 

Path Cost: Very high

Average Time: Very high 


•	Obstacle Density of 70%-90%: 

Path Found: 0% success rate 

Path Cost: N/A 

Average Time: N/A 

## Detailed Observations 

Low Obstacle Densities (10-20%):

The A* algorithm performs optimally, finding paths efficiently with consistent path costs and high success rates. 


Moderate Obstacle Densities (30-50%): 

The success rate drops, and path costs become more variable. The algorithm struggles to find paths in some instances as obstacles increase. 


High Obstacle Densities (60-90%):

The algorithm fails to find paths in most cases. The environment becomes too cluttered, significantly affecting performance.

![alt hi](![image](https://github.com/user-attachments/assets/f1722088-04a5-47e7-af59-39787051fe49)
)

