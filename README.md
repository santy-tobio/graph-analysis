# Graph Analysis Project

## Overview
This project implements various graph analysis algorithms to study the Google Web Graph dataset. The analysis includes connectivity components, shortest paths, clustering coefficients, and several other graph metrics and algorithms.

## Features

### Core Functionality:
- Custom Graph implementation with adjacency list representation
- Connected components analysis
- Shortest path algorithms
- Triangle counting in graphs
- Polygon detection for various sizes
- Clustering coefficient calculation
- Betweenness centrality computation
- PageRank implementation

### Key Metrics Calculated:
- Size of largest connected component: 855,802 vertices
- Number of connected components: 2,746
- Number of triangles: 3,889,771
- Estimated graph diameter: 41
- Average clustering coefficient: 0.367
- Top PageRank and betweenness centrality nodes

## Project Structure
- `graph.py`: Core graph data structure implementation
- `Tp4_Tobio.ipynb`: Main analysis notebook containing all algorithms and results

## Requirements
- Python 3.8+
- NumPy
- Matplotlib
- tqdm
- Jupyter Notebook

## Installation
1. Clone this repository:
```bash
git clone https://github.com/santy-tobio/graph-analysis.git
cd graph-analysis
```

2. Install required packages:
```bash
pip install numpy matplotlib tqdm jupyter
```

## Usage
The project is structured as a Jupyter notebook. To run the analysis:

1. Start Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `graph_analysis.ipynb`
3. Run all cells to see the complete analysis

## Algorithms and Methods

### Connected Components
- Implements DFS-based algorithm to find connected components
- Converts directed graph to undirected for component analysis
- Provides component size distribution

### Shortest Paths
- Implements BFS for unweighted shortest paths
- Estimates all-pairs shortest paths using sampling
- Calculates graph diameter through path analysis

### Triangle Counting
- Efficient algorithm for finding triangles in directed graphs
- Handles both directed and undirected triangle patterns
- Provides total triangle count

### PageRank
- Implements random walk-based PageRank
- Provides ranking of most important vertices
- Includes visualization of PageRank distribution

### Clustering Coefficient
- Calculates local clustering coefficients
- Provides global clustering coefficient
- Analyzes network transitivity

## Results Highlights
- Graph contains 875,713 vertices and 5,105,039 edges
- Largest connected component contains 97.8% of vertices
- High clustering coefficient indicates strong local connectivity
- Power-law distribution in component sizes

## Future Improvements
- Implement more efficient algorithms for large-scale graphs
- Add more graph metrics and analysis tools
- Improve visualization capabilities
- Add support for weighted edges
- Implement parallel processing for large graphs

## Contributing
Feel free to fork this repository and submit pull requests. You can also open issues for bugs or feature requests.

## License
This project is open source and available under the MIT License.
