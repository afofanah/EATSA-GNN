
# EATSA-GNN: Edge-Aware and Two-Stage Attention for Enhancing Graph Neural Networks Based on Teacher-Student Mechanisms for Graph Node Classification

This repository contains the implementation of EATSA-GNN, a novel approach to improve graph neural networks through edge-aware and two-stage attention mechanisms. The model leverages teacher-student frameworks to enhance node classification tasks on graph data.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Model Overview](#model-overview)
- [Experimental Results](#experimental-results)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Graph neural networks (GNNs) offer powerful methods for learning from graph-structured data. The **EATSA-GNN** model enhances traditional GNNs by incorporating edge-aware and two-stage attention, which helps selectively focus on crucial graph components. This combined with teacher-student learning strategies boosts performance on node classification tasks.

### Key Components

- **Edge-Aware Mechanism:** Integrates edge information into the attention process, improving focus on significant node relationships.
- **Two-Stage Attention:** Provides multi-layer attention insights to better capture node importance across graph structures.
- **Teacher-Student Framework:** Enables knowledge distillation from complex models (teachers) to simpler but efficient student models.

## Getting Started

These instructions will help you set up and run the EATSA-GNN model on your local machine.

### Prerequisites

Ensure you have Python 3.11 installed along with the following libraries:

- pyTorch
- pyTorch Geometric
- dgl (if necessary for your dataset)
- networkX
- matplotlib
- scikit-learn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/EATSA-GNN.git
   cd EATSA-GNN
   ```

2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Model Overview

EATSA-GNN builds upon the concept of enhancing node representation learning through targeted attention mechanisms:
- **Data Representation:** Processes graphs like the MUTAG dataset to extract node features.
- **Training Process:** Utilizes a GCN backbone enhanced with two-stage attention to refine focus in prediction tasks.
- **Teacher-Student Interaction:** Facilitates learning efficiencies by transferring knowledge from comprehensive models to lightweight alternatives.

## Citation

@article{Fofanah2024EATSAGNNEA,
  title={EATSA-GNN: Edge-Aware and Two-Stage attention for enhancing graph neural networks based on teacher-student mechanisms for graph node classification},
  author={Abdul Joseph Fofanah and Alpha Omar Leigh},
  journal={Neurocomputing},
  year={2024},
  volume={612},
  pages={128686},
  url={https://api.semanticscholar.org/CorpusID:273438622}
}
Modify dataset paths and hyperparameters as needed within the script.

## Experimental Results

Upon training, the model outputs metrics such as accuracy, precision, and AUC to evaluate performance across training, validation, and test phases. Adjusting model parameters can optimize results based on specific datasets.

## Visualization

The repository provides methods to visualize attention weights using NetworkX, allowing insights into which nodes the model prioritizes. Use these visualizations to interpret model decisions and refine attention strategies further.

## Contributing

Contributions are encouraged, whether they involve feature enhancements, bug fixes, or code optimizations. Please fork the repository and submit a pull request with your contributions.

## License

This project is licensed under the MIT License. See the [LICENSE.md](LICENSE.md) file for details.
MIT License

Copyright (c) 2024 ABDUL JOSEPH FOFANAH AND ALPHA UMAR LEIGH

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

### Final Notes:
- Customize URLs, file paths, and any code examples to suit your specific repository setup.
- Keep the README updated with any changes in project scope or added features.
- Ensure that your `requirements.txt` accurately lists all necessary dependencies for an optimal setup.
