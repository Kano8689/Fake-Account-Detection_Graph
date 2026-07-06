# 🕸️ Multi-Level Fake Account Detection in Social Networks using Graph Centrality and GNNs

An Artificial Intelligence and Graph Machine Learning project that detects suspicious or fake accounts in social networks by combining **Graph Mining Techniques**, **Centrality Measures**, **Community Detection**, **Node Embeddings**, and **Graph Neural Networks (GCNs)**. The system analyzes the structural properties of social networks to identify anomalous users and demonstrates how graph representation learning can improve fake account detection. The implementation is developed in Python using the Facebook Combined Social Network Dataset from the Stanford Network Analysis Project (SNAP).

---

## 🎯 Project Objectives

* Detect fake or suspicious users in a social network.
* Analyze graph structures using graph mining techniques.
* Compute graph centrality measures to identify influential and anomalous nodes.
* Detect communities within the network.
* Generate graph embeddings using Node2Vec.
* Train a Graph Convolutional Network (GCN) for node classification.
* Evaluate model performance using standard classification metrics.
* Visualize network structures, communities, and prediction results.

---

## 📋 Project Requirements

✔ Dataset containing more than **1000 nodes**

✔ At least one **Graph Mining Technique**

✔ At least one **Graph Embedding Method**

✔ Graph Neural Network implementation

✔ Performance Evaluation

✔ Network Visualization

✔ Python Implementation

✔ Source Code, Documentation, and Result Analysis

---

## 📊 Dataset Information

**Dataset Name**

Facebook Combined Social Network Dataset

**Source**

Stanford Network Analysis Project (SNAP)

**Dataset File**

`facebook_combined.txt`

### Dataset Statistics

| Property            |          Value |
| ------------------- | -------------: |
| Nodes (Users)       |           4039 |
| Edges (Connections) |         88,234 |
| Graph Type          |     Undirected |
| Network Type        | Social Network |

The dataset is represented as an edge list where each line contains two node IDs representing a connection (friendship) between users. The dataset satisfies the project requirement of containing more than 1000 nodes.

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Graph Analytics

* NetworkX
* Node2Vec

### Machine Learning

* PyTorch
* PyTorch Geometric
* Graph Convolutional Network (GCN)

### Data Processing

* Pandas
* NumPy

### Data Visualization

* Matplotlib

### Development Environment

* Jupyter Notebook

---

## 🧠 Graph Analytics Workflow

### 1. Data Loading

The Facebook social network dataset is loaded from an edge list file and converted into a graph structure using NetworkX.

### 2. Graph Construction

The edge list is transformed into an undirected graph where:

* Nodes represent users.
* Edges represent friendships or interactions.

This graph representation enables structural analysis and graph-based learning.

---

### 3. Graph Mining Techniques

The project extracts important structural information using graph mining techniques.

#### Degree Centrality

Measures the number of direct connections a user has.

Useful for identifying unusually connected accounts.

#### Betweenness Centrality

Measures how often a node lies on the shortest path between other nodes.

Helps identify bridge nodes connecting different communities.

#### Closeness Centrality

Measures how quickly a node can reach all other nodes.

Useful for identifying peripheral or isolated accounts.

#### Eigenvector Centrality

Measures node importance based on the importance of its neighbors.

Identifies highly influential users in the network.

---

### 4. Community Detection

Community detection groups users with similar interaction patterns.

This project applies modularity-based community detection to identify:

* Dense user communities
* Suspicious cross-community connections
* Isolated user clusters

Community information provides additional structural features for fake account detection.

---

### 5. Node Embedding

Machine learning models cannot directly process graph structures.

Node2Vec converts every node into a numerical feature vector while preserving:

* Local neighborhood relationships
* Global graph structure
* Node similarity

These embeddings become the feature representation used by the Graph Neural Network.

---

### 6. Graph Neural Network (GCN)

A Graph Convolutional Network (GCN) is trained to classify users based on both:

* Graph topology
* Node feature representations

Unlike traditional neural networks, GCNs aggregate information from neighboring nodes, allowing the model to learn complex structural patterns within the social network.

---

## 🔬 Model Training Pipeline

The machine learning workflow consists of:

1. Load Facebook dataset
2. Construct graph
3. Compute centrality measures
4. Detect communities
5. Generate Node2Vec embeddings
6. Create feature matrix
7. Split training and testing data
8. Train Graph Convolutional Network
9. Evaluate model performance
10. Predict fake and genuine accounts

---

## 📈 Evaluation Metrics

The model performance is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score

These metrics measure the effectiveness of the proposed fake account detection system.

---

## 📊 Visualizations

The notebook includes multiple visualizations for better understanding of the network and model performance.

### Network Graph

Visualizes the complete Facebook social network.

### Community Structure

Displays detected communities and user clusters.

### Centrality Analysis

Highlights influential and isolated nodes.

### Training Performance

Shows GCN convergence during training.

### Confusion Matrix

Evaluates classification performance.

### ROC Curve

Illustrates classifier effectiveness.

### Detection Results

Visualizes fake and genuine account predictions.

---

## 📂 Project Structure

```text
Multi-Level-Fake-Account-Detection/
│
├── FraudAccountDetection.ipynb
├── facebook_combined.txt
├── README.md
├── screenshots/
│   ├── network_graph.png
│   ├── communities.png
│   ├── confusion_matrix.png
│   └── roc_curve.png
└── Documentation/
    └── Fake_Account_Detection_Documentation.pdf
```

---

## 🚀 How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/Multi-Level-Fake-Account-Detection.git
cd Multi-Level-Fake-Account-Detection
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib networkx node2vec torch torch-geometric scikit-learn
```

### Run the Notebook

```bash
jupyter notebook FraudAccountDetection.ipynb
```

---

## 📄 Documentation

A detailed project report describing the methodology, graph mining techniques, Graph Neural Network implementation, experimental results, and analysis is included in this repository.

📘 **Project Report:** [Open Project Report (PDF)](https://github.com/Kano8689/Fake-Account-Detection_Graph/blob/main/Fake_Account_Detection_Documentation.pdf)


## 📸 Screenshots

Add your project screenshots here.

```text
screenshots/network_graph.png
screenshots/communities.png
screenshots/confusion_matrix.png
screenshots/roc_curve.png
```

---

## 🎓 Learning Outcomes

This project demonstrates practical knowledge of:

* Graph Data Analytics
* Graph Mining
* Social Network Analysis
* Graph Representation Learning
* Node Embedding (Node2Vec)
* Graph Neural Networks (GCNs)
* Community Detection
* Network Centrality Analysis
* Machine Learning on Graph Data
* AI-based Fake Account Detection

---

## 💼 Applications

* Social Media Security
* Fake Account Detection
* Fraud Detection
* Cybersecurity
* Bot Detection
* Community Analysis
* Recommendation Systems
* Network Intelligence

---

## 👨‍💻 Author

**Krishnam Mavani**

* GitHub: https://github.com/kano8689

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub. It supports future projects in Artificial Intelligence, Graph Machine Learning, Data Science, and Social Network Analytics.
