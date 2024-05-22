# UCL COMP0123 Complex Networks and Web (2023/24)

This repository contains the two major courseworks I completed for my MSc module [COMP0123 Complex Networks and Web](https://www.ucl.ac.uk/module-catalogue/modules/complex-networks-and-web-COMP0123).


## Coursework 1: Analysis of Academic Social Network Data

### Description

This coursework focuses on analyzing a social network of academic authors whose research interests are related to "social networks". The main tasks include data preparation, calculating network properties, and comparing different network models. The analysis covers the author network, a random network, and a Barabási-Albert (BA) network, focusing on metrics like degree distribution, assortativity, and community structure.

### Tasks

1. **Preparation of Network Data**

   - Extract authors with specific research interests and create a giant component network.
   - Generate a random network and a BA network for comparison.

2. **Network Properties Calculation**

   - Average and maximum node degree, degree distribution, and power-law exponent estimation.
   - Nearest neighbor’s average degree and assortative coefficient.
   - Network diameter, average shortest path length, and node betweenness.
   - Rich-club coefficient analysis.
   - Community structure detection and visualization.

3. **Random Network Rewiring**

   - Rewire networks while preserving degree distribution.
   - Compare clustering coefficient, assortative coefficient, giant component size, and average shortest path length between original and randomized networks.

### Tools and Libraries

- Python
- NumPy
- NetworkX
- Seaborn


## Coursework 2: Research Project on Network Science


Project Title: A Network Approach to Image Classification using Community Detection Algorithms and Image Embeddings

### Abstract
This project explores using network community detection for image classification with the MNIST dataset. It constructs image networks via raw pixel values and EfficientNet embeddings, applying the Louvain method for community detection. Results show that image embeddings effectively capture community structures, with classification accuracy comparable to K-Nearest Neighbor (KNN) algorithms.

### Background
Image classification is essential in applications like autonomous driving and medical analysis. Traditional methods like CNNs require significant resources and lack interpretability. This study uses network science and community detection to classify images, representing them as nodes and defining edges based on similarity metrics.

### Research Questions
1. **How can we effectively represent images as a network for analysis?**
   - Investigate methods for embedding images as nodes and establishing edges based on similarity metrics.

2. **What is the performance impact of community detection algorithms on image classification?**
   - Assess the effectiveness of community detection, specifically the Louvain method, compared to traditional methods like KNN.

### Methodology
- **Dataset:** A reduced subset of the MNIST dataset (2,000 training and 500 testing images).
- **Feature Vector Extraction:** Using raw pixel values and EfficientNet embeddings.
- **Edge Definition:** Using cosine and Euclidean distances, constructing networks via distance thresholds or KNN schemes.
- **Community Detection:** Applying the Louvain method with a voting mechanism for label assignment.
- **Model Selection:** Stratified 5-fold cross-validation to select optimal parameters.

### Results
- Models using latent features and cosine distance performed best.
- Community detection models based on latent features achieved high accuracy, comparable to supervised KNN models.

### Tools and Libraries
- Python
- NumPy
- NetworkX
- Scikit-learn
- PyTorch
- Seaborn