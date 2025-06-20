# Butterfly Species Richness Analysis Using Unsupervised Learning

## Overview
This repository contains the implementation and analysis of butterfly species richness using unsupervised learning techniques. The project explores global biodiversity patterns through machine learning approaches to identify ecological clusters and environmental drivers affecting butterfly distribution.

## Abstract
This study applies unsupervised learning techniques including Principal Component Analysis (PCA) and autoencoders to analyze butterfly species richness across 45 diverse global locations. The research identifies key environmental variables affecting species distribution and reveals distinct ecological patterns, with latitude, climate classification, and deforestation emerging as primary drivers of biodiversity.

## Installation

### Prerequisites
- Python 3.8+
- Jupyter Notebook

### Setup
```bash
git clone https://github.com/niharikapatil2306/Butterfly-Species-Richness-Analysis-Using-Unsupervised-Learning.git
cd Butterfly-Species-Richness-Analysis-Using-Unsupervised-Learning
```

## Dataset
- Source: Multi-source environmental and biodiversity databases
- Size: 45 locations × 13 environmental features
- Coverage: Global locations including countries, cities, and topological features
  
### Key Features:
- Climate variables (Köppen-Geiger classification, humidity, temperature)
- Geographic factors (latitude, elevation, area, island status)
- Land use patterns (deforestation, agriculture, urbanization)
- Biodiversity indicators (plant species, butterfly species richness)

## Methodology

### Unsupervised Learning Techniques Used:
- Principal Component Analysis (PCA): Dimensionality reduction and feature importance analysis
- Autoencoders: Neural network-based non-linear dimensionality reduction
- K-means Clustering: Species richness pattern identification (k=3)
- Data Preprocessing: Z-score normalization, mean imputation, one-hot encoding
- Evaluation Metrics: Variance explained, reconstruction loss, silhouette analysis

## Results
- Dimensionality Reduction: Successfully reduced 13D data to 8 key components capturing ~100% variance
- Variance Explanation: First two principal components explain 52.82% of total variance (PC1: 33.74%, PC2: 19.08%)
- Primary Drivers: Latitude, Köppen-Geiger climate classification, deforestation levels
- Model Performance: Autoencoder achieved 0.70 reconstruction loss after 4500 epochs

## Usage

### Running the Analysis
1. Open the Jupyter notebook:
   ```bash
   jupyter notebook main.ipynb
   ```
2. Run cells sequentially to reproduce the analysis
3. Modify parameters as needed for different experiments

## Key Findings
- Climate Impact: Tropical regions show significantly higher species richness (1000+ species) compared to temperate and insular areas
- Geographic Patterns: Strong negative correlation between latitude and species richness, with peak diversity near the equator
- Environmental Drivers: Deforestation, urbanization, and climate classification emerged as critical factors affecting butterfly distribution
- Methodological Insight: Autoencoders captured complex non-linear relationships that traditional PCA methods missed

## Future Work
- Incorporate temporal data to analyze species richness trends over time
- Expand dataset to include more geographic regions and climate zones
- Implement advanced clustering techniques (DBSCAN, hierarchical clustering)
- Develop predictive models for species richness forecasting under climate change scenarios
- Integration with remote sensing data for real-time biodiversity monitoring

## Contributing
This is a research project. For questions or collaboration opportunities, please contact patilniharika2306@gmail.com.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
---

*This project was developed as part of Machine Learning in Sciences I coursework focusing on biodiversity analysis using machine learning techniques.*
