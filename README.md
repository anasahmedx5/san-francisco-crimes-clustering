# San Francisco Crimes Clustering

## Project Overview

This project focuses on analyzing crime incidents in San Francisco using unsupervised learning techniques. By applying clustering algorithms such as **K-Medoids** and **Hierarchical Clustering**, we aimed to discover hidden patterns in the dataset based on features like geographic location, time of occurrence, and crime category. The insights generated can support crime trend analysis and decision-making in public safety and urban planning.

## Design Overview

### Data Preprocessing
- **Dataset**: San Francisco Crime Classification dataset from Kaggle.
- **Sampling**: A random sample of **10,000 rows** was used due to the dataset's large size.
- **Feature Selection**:
  - Location: `X`, `Y`
  - Time: `Hour`, `Day`, `Month`, `Year`
  - Categorical: Encoded `Category`
- **Scaling**: StandardScaler was used to normalize features.
- **Dimensionality Reduction**: PCA (`n_components=2`) was applied for 2D visualization.

### Clustering Algorithms
- **K-Medoids**: Used for its robustness to outliers.
- **Hierarchical Clustering**: Explored nested structure and visualized clusters using dendrograms.
- **Distance Metric**: Euclidean distance after scaling.

## Evaluation

### Visualization
- PCA scatter plots colored by cluster labels
- Hierarchical clustering dendrograms

### Interpretation
- Analyzed patterns in crime locations and timings
- Identified groupings of similar crime incidents

## Key Components

### Libraries Used
- `pandas`: Data manipulation
- `numpy`: Numerical operations
- `matplotlib`, `seaborn`: Visualization
- `scikit-learn`: Scaling, PCA, and clustering utilities
- `scipy`: Hierarchical clustering and dendrogram
- `scikit-learn-extra`: K-Medoids algorithm

### Process
1. Load and preprocess dataset
2. Sample 10,000 entries for performance
3. Scale features and encode categorical data
4. Apply PCA for dimensionality reduction
5. Perform K-Medoids and Hierarchical clustering
6. Visualize and interpret the results

## Algorithms Used
- **K-Medoids Clustering**: Forms clusters based on representative data points (medoids)
- **Hierarchical Clustering**: Builds a tree of nested clusters
- **PCA**: Reduces data to two dimensions for clearer visualization

## Results
- Generated distinct clusters revealing spatial and temporal crime trends
- PCA plots and dendrograms aided in understanding patterns
- Provided insight into potential crime hotspots and time-based patterns

This project illustrates the value of unsupervised learning in uncovering meaningful insights from real-world crime data.
