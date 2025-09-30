# Star Wars Social Network Analysis

## 📌 Overview

This project explores the interactions among characters from the **Star Wars saga** using **Social Network Analysis (SNA)** techniques.
The goal is to study the social network of the characters to highlight hidden structures, the most influential nodes, and emerging communities, leveraging graph theory principles.

## 📂 Dataset

The dataset was built from the scripts of Episodes I–VII and represents relationships between characters based on two criteria:

* **Interactions**: two characters are connected if they appear in the same scene and talk to each other.
* **Mentions**: two characters are connected if they are mentioned in the same scene.

Structure:

* **Nodes** → characters (with name, index, weight, and color)
* **Edges** → connections between characters, weighted by the number of shared scenes

Dataset source: [Star Wars Social Network](https://github.com/evelinag/StarWars-social-network)

## 🛠️ Tools

* **NetworkX** → graph creation and analysis
* **Matplotlib & Seaborn** → data visualization
* **Pandas** → data manipulation

## 🔍 Analyses

The project is organized into several stages:

### 1. Descriptive Analysis

* Basic graph statistics (nodes, edges, density, diameter, clustering coefficient, etc.)
* Network visualization using different layouts:

  * Spring Layout
  * Spiral Layout
  * Kamada-Kawai Layout
  * Circular Layout

### 2. Centrality Analysis

* **Degree Centrality** → most connected characters
* **Betweenness Centrality** → bridge characters connecting communities
* **Eigenvector Centrality** → influence based on connections with influential nodes
* **Closeness Centrality** → accessibility and efficiency of information spread
* Special focus on **Darth Vader** as the most central figure in the network

### 3. Structural Analysis

* **Triads** → groups of three characters
* **Cliques** → fully connected subgraphs
* **K-Core** → cohesive subgraphs based on minimum degree k
* **Ego-Networks** → centered on Luke, Darth Vader, and Rey
* **Group Centrality** → comparing trilogies (prequel, original, sequel)
* **Community Detection** → 7 distinct communities identified via modularity

## 📊 Key Findings

* **Darth Vader** consistently emerges as the most influential character across all centrality measures.
* Different trilogies show different social structures: the prequels have a more collective network, while the original trilogy is focused on a few main characters.
* The network is dominated by a small set of central hubs that act as narrative bridges.
* **7 main communities** were identified, corresponding to factions, political groups, or military affiliations.

## 👥 Authors

Project developed for the **Data science** course at *Università Politecnica delle Marche*.

* Walter Di Sabatino
* Alessandra D’Anna
* Agnese Bruglia