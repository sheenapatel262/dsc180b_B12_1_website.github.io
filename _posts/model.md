---
title:  "Model"
mathjax: true
layout: post
categories: media
---

## Summary: Construction of Models

For traffic speed prediction, we adopt the **Spatial-Temporal Graph Attention Network (ST-GAT)** proposed by Zhang, Yu, and Liu (2019). ST-GAT efficiently integrates spatial relationships and temporal variations within the network, enabling precise traffic forecasting. Two variants of ST-GAT are introduced: **ST-GAT Single Edge** and **ST-GAT Edge Type**.

### ST-GAT Single Edge:

- Utilizes a **Graph Attention (GAT)** layer to aggregate neighboring node features.
- Enhances traditional **Graph Convolutional Networks (GCN)** with self-attention mechanisms.
- Employs **Long Short-Term Memory (LSTM)** layers for capturing temporal characteristics.
- Employs a **linear output layer** for generating traffic speed forecasts.

### ST-GAT Edge Type:

- Segregates graph signals based on edge types to discern their importance.
- Applies GAT layer independently to each edge type for unique feature embeddings.
- Utilizes LSTM layers for capturing temporal dependencies.
- Employs a linear output layer for traffic speed prediction.

## Experiments:

- **Datasets:** Construct six distinct graphs representing different highway networks.
- **Setup:** Split dataset into training, validation, and test subsets.
- **Model Initialization:** Initialize models for training with specific configurations.
- **Evaluation:** Evaluate model performance using root mean squared error (RMSE), mean absolute error (MAE), and mean absolute percent error (MAPE) metrics.

Overall, the ST-GAT models demonstrate effective traffic speed prediction capabilities, as evidenced by their performance on the testing set.
