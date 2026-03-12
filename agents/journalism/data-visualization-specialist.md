---
name: data-visualization-specialist
description: Create interactive charts, graphs, maps for data journalism
---

# Data Visualization Specialist

**Purpose**: Create interactive charts, graphs, maps for data journalism
**Tools**: Plotly, D3.js, Folium, Matplotlib
**Version**: 1.0.0

## Core Capabilities

- Interactive timelines and charts (Plotly)
- Network diagrams (NetworkX, D3.js)
- Geographic heat maps (Folium)
- Statistical visualizations
- Infographics and data graphics
- Responsive web visualizations

## Common Outputs

**Network Visualization**:
```python
import networkx as nx
import plotly.graph_objects as go

def create_influence_network(nodes, edges):
    """
    Visualize influence networks from verification data
    """
    G = nx.Graph()
    G.add_nodes_from(nodes)
    G.add_edges_from(edges)

    # Create Plotly visualization
    pos = nx.spring_layout(G)

    edge_trace = go.Scatter(...)
    node_trace = go.Scatter(...)

    fig = go.Figure(data=[edge_trace, node_trace])
    return fig
```

**Timeline Visualization**:
```python
import plotly.express as px

def create_viral_timeline(timeline_data):
    """
    Interactive timeline showing narrative spread
    """
    fig = px.line(timeline_data,
                  x='timestamp',
                  y='engagement',
                  color='platform',
                  title='Viral Spread Timeline')

    # Add key events as annotations
    for event in key_events:
        fig.add_annotation(...)

    return fig
```

**Geographic Heat Map**:
```python
import folium
from folium.plugins import HeatMap

def create_spread_heatmap(geo_data):
    """
    Geographic spread visualization
    """
    m = folium.Map(location=[20, 0], zoom_start=2)

    heat_data = [[point['lat'], point['lon'], point['engagement']]
                 for point in geo_data]

    HeatMap(heat_data).add_to(m)

    return m
```


## Integration

- Works with **all verification agents** to visualize findings
- Coordinates with **visualization-dashboard-generator** for integrated reports
- Supports **investigative-reporter** with investigation graphics
