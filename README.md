# Network Analysis with Python

This workshop introduces network analysis with Python and NetworkX. We focus on representing relationships as networks, constructing graphs from data, visualizing network structure, and exploring connections between nodes.

Networks provide a useful way to represent relationships between researchers and organizations through publications, patents, collaborations, and citations. In each case, entities can be represented as **nodes** and relationships between those entities as **edges**.

The workshop begins by constructing a small network manually so that the basic components of a graph are visible. We then build a research collaboration network from tabular data and use NetworkX to explore degree, connectivity, shortest paths, alternative paths, and attributes associated with relationships.

The examples use small fictional datasets so that the network structure remains easy to inspect. The same methods can later be applied to larger datasets retrieved from APIs, databases, and other sources.

## Table of Contents

- [Objectives](#objectives)
- [Prerequisites](#prerequisites)
- [NetworkX](#networkx)
- [Workbooks](#workbooks)
  - [NetworkX Introduction](#networkx-introduction)
  - [Building a Collaboration Network from Data](#building-a-collaboration-network-from-data)
- [Relationship to the Workshop Series](#relationship-to-the-workshop-series)
- [Additional Resources](#additional-resources)

## Objectives

By the end of this workshop, participants will be able to:

- Explain the difference between nodes and edges
- Create an undirected graph with NetworkX
- Add nodes, edges, and attributes to a graph
- Build a graph from tabular relationship data
- Visualize a network with NetworkX and Matplotlib
- Find paths between nodes
- Use attributes to add information about nodes and relationships

## Prerequisites

Some previous experience with Python is helpful but extensive programming experience is not required.

The workshop uses Jupyter notebooks running Python. The second workbook also uses pandas to represent a small table of collaboration data.

Participants who want to run the examples will need:

- Python
- Jupyter Notebook or JupyterLab
- NetworkX
- pandas
- Matplotlib

No previous experience with graph theory, network analysis, or NetworkX is required.

## Instructor

Geoffrey Boushey is a computational and research data science specialist at UCSF and a member of the Library's Data Science and Open Scholarship team. Geoff teaches courses and provides consultations on foundational programming, data analysis, and AI techniques including Python, SQL, Unix, and Version Control.

## Workbooks

### NetworkX Introduction

#### [NetworkX-Introduction.ipynb](https://github.com/UCSF-DSOS/Network-Graphs/blob/main/NetworkX-Introduction.ipynb)

This workbook introduces network graphs by constructing a small research collaboration network from first principles.

Participants create an empty graph, add fictional researchers as nodes, store information about researchers as node attributes, and add collaboration relationships as edges.

The completed graph is visualized with NetworkX and Matplotlib. The example also introduces neighbors, node degree, and graph connectivity.

The emphasis is on making the structure of the graph visible before automating graph construction from data.

### Building a Collaboration Network from Data

#### [NetworkX-Collaboration-From-Data.ipynb](https://github.com/UCSF-DSOS/Network-Graphs/blob/main/NetworkX-Collaboration-From-Data.ipynb)

This workbook moves from manually constructing a graph to building one from structured data.

A small pandas DataFrame represents fictional research collaborations. Each row describes a relationship between two researchers, and the notebook uses those rows to construct the network automatically. Collaboration topics are stored as edge attributes.

The workbook then uses the network to explore questions such as:

- Which researchers have the most direct collaborators?
- What is a shortest path between two researchers?
- What alternative paths connect two researchers?
- What collaboration topics occur along a path?

The underlying graph model is the same as in the first workbook. The difference is that the nodes, edges, and attributes are now constructed from data.

## Relationship to the Workshop Series

This workshop is part of a broader UCSF Library curriculum on computational data and document analysis with Python, SQL, machine learning, and AI.

Network analysis provides another way to work with structured data by focusing on relationships rather than individual observations.

The [Research and Patent Landscape Informatics](https://github.com/UCSF-DSOS/Research-Patent-Landscape-Workshop) workshop series applies the methods introduced here to live research and patent data.

In those examples:

- OpenAlex publication data is used to construct researcher collaboration networks based on coauthorship
- USPTO patent application data is used to construct inventor collaboration networks based on co-inventorship

For this workshop, we will use test data to build and explore NetworkX for analyzing graphs, including shortest path and alternative paths between nodes to explore relationships. 

## Additional Resources

- [NetworkX](https://networkx.org/)
- [Matplotlib](https://matplotlib.org/)
- [pandas](https://pandas.pydata.org/)
