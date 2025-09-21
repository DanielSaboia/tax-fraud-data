# tax-fraud-data
This repository provides datasets and supporting documentation related to the study of **graph-based tax fraud detection**.   The data are organized into processed metrics and illustrative samples that allow full reproducibility of the analyses presented in the associated article.

## CSV File Structure

The graph dataset is composed of four CSV files, each storing a specific part of the structure:

* **`graphs_info.csv`**
  Contains the global metadata of each graph.

  * `id_graph`: unique graph identifier
  * `target`: label associated with the graph (e.g., 0 or 1)

* **`graph_nodes.csv`**
  Maps the nodes that belong to each graph.

  * `id_graph`: graph identifier
  * `node_id`: unique identifier of the node within the graph

* **`nodes_attributes.csv`**
  Stores the attributes of the nodes.

  * `id_graph`: graph identifier
  * `node_id`: node identifier
  * `feature`: original feature value associated with the node
  * `norm_value`: normalized value (via MinMaxScaler) of the node feature

* **`edges_attributes.csv`**
  Records the edges and their attributes.

  * `id_graph`: graph identifier
  * `u`: source node of the edge
  * `v`: target node of the edge
  * `feature_rel`: feature associated with the edge

---

👉 Do you want me to also prepare this in a **Markdown table format** (columns vs. description) so it looks more polished in the README?
