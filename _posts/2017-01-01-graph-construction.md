---
title:  "Graph Construction"
layout: post
---
Explore the diverse representations of highway networks through distinct graph structures, each tailored with unique **edge connections** and **node features**. Dive into the dynamics of traffic flow across various time frames within a unified structural framework.


## Nodes
Explore the intricacies of highway network analytics by integrating sensor node data and constructing feature vectors to capture the state and dynamics of sensors within specific time frames:

- **Speed Window**: Captures dynamic speed variations by utilizing a window of previous aggregated speeds from specific time intervals. 

- **Lane Count**: Identifies the constant number of lanes adjacent to each sensor as a critical factor for understanding traffic flow dynamics and bottleneck phenomena. 

- **Day of Week**: Helps in understanding how traffic patterns vary throughout the week, considering factors like weekday rush hours and weekend leisure travel.

- **Hour of Day**: Incorporates the time of day, using a sinusoidal and cosine transformation to capture the cyclical nature of traffic patterns, notably during rush hours. 

## Edges
Dive into the spatial dynamics of highway networks through a comprehensive understanding of edge connections:

#### Type 1: Sequential Linkage
- **Linear Representation**: Establish direct connections between each sensor and its immediate neighbors along the same highway.
- **Straightforward Connectivity**: This type of edge ensures a sequential linkage, portraying the immediate spatial relationships within the network.

#### Type 2: External Influences
- **Capturing External Dynamics**: Acknowledge potential influences from sensors external to a given highway, accounting for traffic diversions and alternate routes.
- **Nuanced Representation**: These edges provide insights into traffic patterns influenced by external factors, enhancing the understanding of inter-highway dynamics.

#### Type 3: Long-Range Dependencies
- **Capturing Extended Interactions**: Grasp the impact of traffic dynamics originating from distant locales within a designated highway.
- **Efficient Representation**: Utilize skip connections to capture long-range interactions directly, mitigating the challenges posed by extensive propagation through intermediate sensors.
  
<center>
<img src= "../assets/edge_types.png" width= 500>
</center>
