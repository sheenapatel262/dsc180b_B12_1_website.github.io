---
title: "Project Overview"
layout: post
---

**Traffic Flow Prediction: Enhancing Commuter Experience**

In a world where automobiles are ubiquitous, traffic congestion remains an enduring challenge, whether triggered by accidents or rush hour bottlenecks. While complete eradication of traffic may be unattainable due to the sheer volume of vehicles, we can certainly enhance our ability to predict traffic flow more effectively.

Existing platforms like Apple Maps or Waze rely on techniques such as Random Forest classifiers or historical averages, which often fail to account for long-range traffic effects. Consequently, by the time drivers are alerted to heavy traffic, they're already ensnared within it.

Our proposition? A novel approach utilizing graph neural networks (GNNs), integrating time series and geospatial analysis methodologies to bolster traffic flow prediction. GNNs excel in handling long-range interactions, holding promise for early traffic identification. Beginning with a focused examination of recent traffic sensor data in San Diego, our endeavor aims to forecast traffic flow, comparing predictions against actual traffic to gauge model efficacy.

Our ultimate ambition is to craft a versatile GNN model applicable across major freeways, revolutionizing traffic prediction by amalgamating GNN prowess with nuanced features like lane numbers and nonlinear message passing. The envisioned outcome? Empowering drivers with timely, accurate information to navigate congested routes more efficiently.

**Exploring Graph Neural Networks**

Graph neural networks (GNNs) represent a revolutionary machine learning data structure comprising nodes holding information and edges containing associative pieces of data. These structures offer immense flexibility, serving as both data organization tools and single data points linked to form networks. Leveraging these relationships, GNNs enhance classification, prediction, and other algorithmic applications, marking a significant advancement in deep learning.

**Capstone Project Overview**

During the initial phase of our capstone project, we delved into various GNN models, including GIN, GCN, GATv2, and GraphGPS, assessing their efficacy in node and graph classification tasks. Employing datasets from the PyTorch Geometric library, our empirical investigations aimed to unveil the strengths and limitations of these architectures, aiding us in selecting the most suitable model for our application context.

Initially inspired by Rose Yu’s seminal work on traffic forecasting, our project encountered challenges in implementing Diffusion Convolutional Recurrent Neural Network (DCRNN) models, prompting a pivot towards leveraging existing GNN knowledge. Drawing insights from published articles and securing sensor data from major highway systems, we embarked on creating a Spatio-Temporal Graph Attention Network (ST-GAT) to predict traffic flow patterns across San Diego County's primary highways.

**Future Directions**

Our project trajectory involves exploring diverse edge relationships between sensor data points and integrating a myriad of features to enhance traffic flow prediction accuracy. While our baseline model adopts a simplistic linear graph framework, our final iteration will delve into more intricate features, including a time series component and Euclidean distance connectivity, promising to refine traffic prediction methodologies for optimized commuter experiences.
