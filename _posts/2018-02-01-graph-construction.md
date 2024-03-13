---
title:  "Graph Construction"
layout: post
---
Explore the diverse representations of highway networks through distinct graph structures, each tailored with unique edge connections and node features. Dive into the dynamics of traffic flow across various time frames within a unified structural framework.


## Nodes
- **Sensor Representation**: Each node embodies a sensor strategically positioned along the highway network, serving as a crucial data point for analysis.
- **Feature Vector Construction**: Construct feature vectors for nodes, encapsulating a plethora of attributes that depict the sensor's state within specific time frames.
<center>
<img src="../assets/sensor-map.png" width= 250>
</center>

### Speed Window
- **Temporal Dynamics Integration**: Capture the essence of highway temporal dynamics through the creation of speed windows for each node.
- **Window of Insight**: These windows, spanning a range of time, encapsulate average speeds, offering a holistic view of speed variations over time.

### Lanes, Weekday, Hour
- **Additional Influential Features**: Identify and incorporate features such as lane count, day of the week, and hour of the day into node feature vectors.
- **Comprehensive Insight**: Enhance the depth of analysis by integrating features that reflect varying traffic patterns across different days and times.

## Edges
Dive into the spatial dynamics of highway networks through a comprehensive understanding of edge connections:

### Type 1: Sequential Linkage
- **Linear Representation**: Establish direct connections between each sensor and its immediate neighbors along the same highway.
- **Straightforward Connectivity**: This type of edge ensures a sequential linkage, portraying the immediate spatial relationships within the network.

### Type 2: External Influences
- **Capturing External Dynamics**: Acknowledge potential influences from sensors external to a given highway, accounting for traffic diversions and alternate routes.
- **Nuanced Representation**: These edges provide insights into traffic patterns influenced by external factors, enhancing the understanding of inter-highway dynamics.

### Type 3: Long-Range Dependencies
- **Capturing Extended Interactions**: Grasp the impact of traffic dynamics originating from distant locales within a designated highway.
- **Efficient Representation**: Utilize skip connections to capture long-range interactions directly, mitigating the challenges posed by extensive propagation through intermediate sensors.
