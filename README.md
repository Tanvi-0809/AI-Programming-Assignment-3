AI Programming Assignment 3

Name: Tanvi Gajula  
Roll Number: SE24UCSE025  
Course: Artificial Intelligence  


Overview

This repository contains the implementation of Assignment 3 in Artificial Intelligence.  
The assignment covers both theory and programming based on uninformed search, informed search, heuristics, Dijkstra’s algorithm, and UGV path planning in static and dynamic obstacle environments.

The repository is divided into three major programming modules and one theory section.


Theory Topics Covered

The theory section includes the following topics:

1. Comparison of Uninformed Search Techniques  
   - Breadth-First Search  
   - Uniform-Cost Search  
   - Depth-First Search  
   - Depth-Limited Search  
   - Iterative Deepening Search  
   - Bidirectional Search  

2. Informed Search Techniques and Applications  
   - Greedy Best-First Search  
   - Best-First Search  
   - Dijkstra’s Algorithm  
   - A* Algorithm  
   - Beam Search  
   - Recursive Best-First Search (RBFS)  
   - Iterative Deepening A* (IDA*)  
   - Weighted A*  

3. Heuristics  
   - Satisficing Search  
   - Inadmissible Heuristic  
   - Formulating a heuristic for a search problem  
   - Generating heuristics from subproblems  


1. Dijkstra Algorithm for Indian Cities

**Folder:** `Dijkstra_India_Cities`
Objective
To implement Dijkstra’s Algorithm, also known as Uniform-Cost Search in AI, to find the shortest path between Indian cities using road distances.

Description
This program models major Indian cities as nodes in a weighted graph, where the road distances between them are edge costs.  
The user provides a start city and a goal city, and the program computes:

- shortest path
- total distance
- visited nodes

Files
- `dijkstra_india.py`
- `cities_distances.csv`
- `README.md`

Run
```bash
cd Dijkstra_India_Cities
python3 dijkstra_india.py

2. UGV Navigation with Static Obstacles

Folder: UGV_Static_Obstacles

Objective

To design an algorithm that allows an Unmanned Ground Vehicle (UGV) to navigate through a 70x70 grid battlefield containing known static obstacles.

Description

The battlefield is represented as a grid. Obstacles are generated randomly with three density levels:
	•	low
	•	medium
	•	high

The UGV must move from the start node to the goal node while avoiding obstacles and following the shortest path.

This module uses the A* search algorithm for path planning.

Measures of Effectiveness
	•	path length
	•	nodes expanded
	•	obstacle density impact

Files
	•	ugv_static.py
	•	README.md

Run

cd UGV_Static_Obstacles
python3 ugv_static.py


3. UGV Navigation with Dynamic Obstacles

Folder: UGV_Dynamic_Obstacles

Objective

To make the UGV navigate in an environment where obstacles are dynamic and not completely known in advance.

Description

This module extends the static obstacle problem.
The UGV initially plans a path using A* search. While moving, new obstacles may appear. If the planned path becomes blocked, the UGV replans from its current position to the goal.

This demonstrates dynamic replanning in a changing environment.

Measures of Effectiveness
	•	path length
	•	nodes expanded
	•	number of replans
	•	mission success/failure
	•	obstacle density impact

Files
	•	ugv_dynamic.py
	•	README.md

Run

cd UGV_Dynamic_Obstacles
python3 ugv_dynamic.py


