# Customer Segmentation with K-Means Clustering

This project demonstrates how to use K-Means clustering to segment retail card customers based on their income and spending score. By following this approach, you can uncover distinct customer groups that share similar characteristics, enabling targeted marketing and customer engagement strategies.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Analysis Steps](#analysis-steps)
- [Results and Insights](#results-and-insights)
- [Conclusions](#conclusions)
- [Future Work](#future-work)

## Project Overview

The goal of this project is to perform customer segmentation using K-Means clustering, a popular unsupervised machine learning algorithm. By clustering customers based on their income and spending score, the project aims to identify groups with similar behaviors, providing actionable insights for customer relationship strategies.

## Dataset

The dataset used in this project contains customer demographic and spending data, including:
- **CustomerID**: Unique identifier for each customer
- **Gender**: Customer's gender (Male/Female)
- **Age**: Customer's age
- **Income**: Annual income of the customer
- **Spending Score**: Score assigned based on customer spending habits

This dataset is ideal for demonstrating customer segmentation techniques with K-Means clustering.

## Installation

To run this project, you'll need Python and the following libraries:

- `pandas`: Data manipulation and analysis
- `matplotlib`: Data visualization
- `seaborn`: Statistical data visualization
- `scikit-learn`: Machine learning library for clustering

Install the required libraries using:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

## Project Structure

- `data/`: Folder containing the dataset (if applicable)
- `notebook.ipynb`: Jupyter Notebook with the code and analysis
- `README.md`: Project documentation
- `images/`: Folder with images or visualizations used in the project (optional)

## Analysis Steps

1. **Data Preparation**
   - Load and inspect the dataset.
   - Explore basic summary statistics to understand the data distribution.

2. **Data Preprocessing**
   - Select relevant features (`Income` and `Spending Score`).
   - Standardize the data to ensure features are on a similar scale for effective clustering.

3. **Determining the Optimal Number of Clusters**
   - Use the Elbow Method, Silhouette Score, and Calinski-Harabasz Score to determine the best value for \( K \) (number of clusters).

4. **Applying K-Means Clustering**
   - Run the K-Means algorithm with the optimal \( K \) value.
   - Assign each customer to a cluster based on their similarity to the cluster centroids.

5. **Evaluating and Visualizing Clusters**
   - Analyze cluster sizes and interpret each cluster’s characteristics.
   - Visualize clusters using scatter plots with centroid labels.

6. **Analyzing and Interpreting Cluster Assignments**
   - Encode the `Gender` feature for additional insights.
   - Calculate summary statistics for each cluster to understand demographic and spending behavior.

7. **Extracting Actionable Insights**
   - Propose strategies based on cluster characteristics, such as targeting high-income, low-spending customers or monitoring high-spending, low-income customers.

## Results and Insights

This clustering analysis revealed five unique customer segments:
- **Cluster 0**: Low income, low spending.
- **Cluster 1**: High income, low spending.
- **Cluster 2**: Low income, high spending.
- **Cluster 3**: High income, high spending.
- **Cluster 4**: Average income and spending.

These insights can be used to develop tailored marketing strategies and improve customer relationship management.

## Conclusions

K-Means clustering is an effective method for customer segmentation. This project shows how clustering can uncover meaningful patterns in customer data, providing valuable insights for targeted engagement.

## Future Work

Potential extensions of this project include:
- Experimenting with other clustering algorithms (e.g., hierarchical clustering).
- Adding more customer features for enhanced segmentation.
- Developing a customer segmentation dashboard for real-time insights.

## License

This project is open-source and available under the MIT License. Feel free to modify and use the code as needed.

---

This README provides a structured overview of the project, guiding users from setup to the results and insights obtained from the clustering analysis.