# Social Network Manager

## Overview

Social Network Manager is a **C++ based social network analysis system** that models users and their relationships using **graph data structures**.
In this project, **users are represented as nodes** and **connections between users are represented as edges**.

The system performs advanced network analysis including:

* Influencer detection
* Community detection
* Connection recommendation
* Graph visualization

The project demonstrates practical use of **Data Structures and Algorithms (DSA)** in analyzing complex social networks.

---

## Features

### User Management

* User registration and login system
* User information stored in CSV files
* Dynamic addition of new users

### Connection Management

* View existing connections
* Add new connections
* Remove connections
* Smart connection recommendations

### Social Network Analysis

The system calculates several important **network metrics**:

* **PageRank** – Identifies influential users in the network
* **Betweenness Centrality** – Finds users that act as bridges between communities
* **Closeness Centrality** – Determines how quickly a user can reach others

### Community Detection

Users are grouped into communities based on:

* Branch
* Category
* Connection structure

### Graph Visualization

The network is visualized as a **graph image** using Graphviz.

Each community is color coded and connections between users are displayed.

---

## Technologies Used

* **C++**
* **Graph Data Structures**
* **Adjacency Matrix**
* **Breadth First Search (BFS)**
* **PageRank Algorithm**
* **Betweenness Centrality**
* **Closeness Centrality**
* **Jaccard Similarity (for recommendations)**
* **OpenMP (Parallel Processing)**
* **Graphviz (Graph Visualization)**

---

## Project Structure

```
social_network_manager
│
├── cpp files
│   ├── adjacency_matrix.cpp
│   ├── connection_handler.cpp
│   ├── connection_manager.cpp
│   ├── graph_visualizer.cpp
│   ├── login_manager.cpp
│   ├── main.cpp
│   └── print_utilities.cpp
│
├── header files
│   ├── adjacency_matrix.h
│   ├── connection_handler.h
│   ├── connection_manager.h
│   ├── graph_visualizer.h
│   ├── login_manager.h
│   ├── print_utilities.h
│   └── user.h
│
├── png_graphs
│
├── user_data.csv
├── build.bat
└── README.md
```

---

## Algorithms Used

### 1. PageRank

Used to determine the **most influential users** in the network.

### 2. Betweenness Centrality

Identifies nodes that act as **bridges between communities**.

### 3. Closeness Centrality

Measures how quickly a user can reach other users in the network.

### 4. Breadth First Search (BFS)

Used for graph traversal and shortest path calculations.

### 5. Community Detection

Users are grouped into communities based on **connection density and attributes**.

### 6. Jaccard Similarity

Used for **connection recommendation** by comparing user attributes.

---

## Installation

### Prerequisites

Install:

* **Git**
* **C++ Compiler (g++ / MinGW)**
* **Graphviz**

Download Graphviz:

https://graphviz.org/download/

---

## How to Run the Project

### 1. Clone the Repository

```
git clone https://github.com/yourusername/social_network_manager.git
```

### 2. Navigate to the Project Folder

```
cd social_network_manager
```

### 3. Build the Project

```
.\build.bat
```

### 4. Run the Program

```
.\build\program.exe
```

---

## Program Workflow

```
User Login / Registration
        ↓
Load Users from CSV
        ↓
Construct Social Network Graph
        ↓
Compute Network Metrics
        ↓
Detect Communities
        ↓
Recommend New Connections
        ↓
Visualize Network Graph
```

---

## Output

The program generates:

* **Top Influencers**
* **Detected Communities**
* **Recommended Connections**
* **Network Graph Visualization**

Graph images are stored in:

```
png_graphs/
```

Example output file:

```
updated_social_network_graph.png
```

---

## Applications

This system can be applied in:

* Social media analytics
* Marketing influencer detection
* Recommendation systems
* Network analysis
* Community detection in large networks

