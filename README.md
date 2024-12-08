# Customer Segmentation for Online Gift Store

This project focuses on segmenting customers of an online gift store using machine learning techniques. The goal is to understand customer behavior and create targeted strategies for different customer segments based on their purchasing patterns.

## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Data Description](#data-description)
- [Clustering Models](#clustering-models)
- [Preprocessing](#preprocessing)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Project Overview

In this project, we aim to cluster customers based on their **Recency**, **Frequency**, and **Monetary (RFM)** values using clustering algorithms like **KMeans** and **DBSCAN**. These clusters will help categorize customers into segments such as loyal, potential, new, dormant, or lost customers.

## Problem Statement

### Business Problem
The objective is to segment the store's customers and define strategies for engaging with each segment.

### Technical Problem
As a data scientist, you will build a machine learning model to classify customers based on their transaction frequency, amount spent, and recency of their last purchase. The primary objective is to create meaningful customer segments that can help guide business decisions.

## Data Description

The dataset contains transaction records from an online gift store. The columns in the dataset include:

- **InvoiceNo**: Invoice number (unique for each transaction).
- **StockCode**: Product code (unique for each product).
- **Description**: Product name.
- **Quantity**: Number of units bought in a transaction.
- **InvoiceDate**: Date and time of the transaction.
- **UnitPrice**: Price per unit of the product.
- **CustomerID**: Unique customer ID.
- **Country**: Customer's country.

## Clustering Models

This project uses clustering techniques to group customers into distinct segments:

- **KMeans**: A clustering algorithm that assigns customers to a predefined number of clusters.
- **DBSCAN**: A density-based algorithm that identifies clusters of varying shapes and sizes.

The best model will be selected based on silhouette scores, and customer segments will be interpreted accordingly.

## Preprocessing

Before applying clustering models, the data undergoes several preprocessing steps, such as handling missing values, scaling numerical features (e.g., using **StandardScaler** or **MinMaxScaler**), and encoding categorical variables.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/yourprojectname.git
    cd yourprojectname
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Data Loading**: Load the customer transaction data from a CSV file.
   
2. **Data Preprocessing**: Clean and preprocess the data by handling missing values, normalizing numerical features, and encoding categorical variables.

3. **Clustering**: Apply **KMeans** and **DBSCAN** clustering algorithms to segment customers based on RFM metrics.

4. **Evaluation**: Use silhouette scores to evaluate the clustering performance and interpret the results.

5. **Analysis**: Analyze the customer segments based on the characteristics of each cluster.

Run the analysis using:

```bash
python segmentation_analysis.py
