#Country Socio-Economic Data Analysis: Dimensionality Reduction and Clustering

This project uses Python and fundamental machine learning techniques (Dimensionality Reduction and Clustering) to analyze global socio-economic indicators and group countries based on their development status.

The workflow involves initial data exploration, feature scaling, reducing the complexity of the data, and finally applying clustering algorithms to identify natural groupings among nations.

- Prerequisites
To reproduce this project, you need a Python 3 environment. The required packages are listed in requirements.txt.


Install Dependencies:
Use the provided requirements.txt file to install all necessary Python libraries.

Bash
pip install -r requirements.txt
-> Data
The project requires a dataset named Country-data.csv.

Expected Location: ../data/Country-data.csv (You will need to create a data directory one level up from where the notebooks are located and place the CSV file inside it).

The dataset is expected to contain socio-economic features like child_mort, exports, health, imports, income, inflation, life_expec, total_fer, and gdpp.

Project Files
The analysis is structured into two main Jupyter Notebooks:

	                                                         
File Name:: dimensionality_reduction_countrydata.ipynb	
Description	Key:: Focuses on exploratory data analysis, feature scaling, and reducing the data's complexity for better visualization and model performance.	
Techniques:: StandardScaler, PCA, t-SNE


File Name:: clustering_countrydata.ipynb	
Description	Key:: Applies clustering algorithms to the scaled and reduced data to identify distinct groups of countries (e.g., developed, developing).	
Techniques:: K-Means, DBSCAN, Silhouette Analysis


How to Run
Ensure you have set up your environment and placed the data file correctly.

Start the Jupyter Notebook server:

Bash
jupyter notebook
Open and run the notebooks in the following order:

dimensionality_reduction_countrydata.ipynb: Run all cells to process the data and understand the underlying structure.

clustering_countrydata.ipynb: This notebook imports and re-runs the necessary data preprocessing steps (scaling, PCA/t-SNE) and then performs the clustering analysis.