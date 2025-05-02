# Enzyme and Protein Graph Classification using Hierarchical DiffPool

This project implements graph classification on biological datasets (Enzymes and Proteins) using the **Hierarchical DiffPool** architecture from the Deep Graph Library (DGL) and PyTorch.

## 🔬 Project Overview

The goal of this project is to classify biological graphs—specifically **enzyme** and **protein** structures—using a deep learning model capable of learning hierarchical representations: **DiffPool**. 

We leverage the TU Dataset (from [TUDataset](https://chrsmrrs.github.io/datasets/docs/datasets/)) which provides standard benchmark graphs for classification tasks.

### 📁 Datasets Used
- **ENZYMES**: Graphs representing protein tertiary structures for 6 enzyme classes.
- **PROTEINS**: Graphs representing proteins with nodes as secondary structure elements and edges as spatial closeness.

## 🧠 Model: Hierarchical DiffPool

**DiffPool** is a graph pooling method that generates hierarchical representations of graphs. Unlike simple pooling, DiffPool learns to cluster nodes into sets, enabling more expressive graph embeddings.

### Model Features
- Multi-layer GNN encoder
- Differentiable pooling layers
- Final MLP classifier for graph-level prediction
- Node features and edge connectivity preserved through the DGL pipeline

## 🚀 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/graph-diffpool-enzymes.git
cd graph-diffpool-enzymes
