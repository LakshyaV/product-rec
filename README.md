# KONEK Product Recommmendation

## Overview

This repository contains a suite of AI-driven models and techniques designed for enhancing recommendation systems and data analysis. The project leverages machine learning models to provide actionable insights and recommendations based on user cart data and past purchase trends.

## Key Components

### Current Cart Analysis
- **Word2Vec Model**: 
  - **Description**: Word2Vec is a neural network-based model that transforms items into vector representations. These vectors capture semantic relationships between items, allowing the model to find similar products by measuring vector similarity.
  - **How It Works**: Trains on item descriptions or attributes to generate dense vector embeddings. Similar items are identified by comparing vector distances in the embedding space, enabling the recommendation of products with analogous features.

### Item Set Discovery
- **FP-Growth Algorithm**: 
  - **Description**: FP-Growth (Frequent Pattern Growth) is an efficient algorithm for mining frequent item sets and association rules from transaction data. It is known for its performance and scalability in large datasets.
  - **How It Works**: Constructs a compact data structure called an FP-tree to represent itemsets. The algorithm recursively mines this tree to find frequent itemsets by leveraging prefix paths. This helps in discovering combinations of items that frequently appear together in transactions.

### Past Cart Analysis
- **LSTM (Long Short-Term Memory)**: 
  - **Description**: LSTM is a type of recurrent neural network (RNN) designed to learn and remember long-term dependencies in sequential data. It is particularly useful for analyzing time-series data and user behavior patterns.
  - **How It Works**: Uses memory cells and gating mechanisms to capture long-term dependencies in historical cart data. This enables the model to identify trends, seasonal variations, and sequential patterns in user purchase history.

- **Neural Collaborative Filtering**:
  - **Description**: Neural Collaborative Filtering (NCF) is a model that combines matrix factorization with neural networks to predict user preferences. It captures complex interactions between users and items.
  - **How It Works**: Utilizes neural networks to learn latent features from user-item interaction data. The network processes these features to predict the likelihood of user preferences for unseen items, improving recommendation accuracy.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
