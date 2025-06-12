# Customer Segmentation using K-Means Clustering

This project demonstrates customer segmentation using the K-Means clustering algorithm in Python. The goal is to group customers based on their characteristics, primarily focusing on 'Annual Income' and 'Spending Score' from a sample mall customer dataset.

## Project Structure

- `Mall_Customers.csv`: The dataset containing customer information.
- `customer_segmentation.ipynb` (or similar): The Jupyter Notebook containing the code for data loading, exploration, preprocessing, K-Means clustering, and visualization.

## Dataset

The dataset used is `Mall_Customers.csv`. It typically contains the following columns:

- `CustomerID`: Unique identifier for each customer.
- `Gender`: The gender of the customer.
- `Age`: The age of the customer.
- `Annual Income (k$)`: The annual income of the customer in thousands of dollars.
- `Spending Score (1-100)`: A score assigned by the mall based on customer behavior and spending habits.

## Dependencies

The project requires the following Python libraries:

- pandas: For data manipulation and analysis.
- numpy: For numerical operations.
- matplotlib: For data visualization.
- seaborn: For enhanced data visualization.
- scikit-learn: For K-Means clustering and data scaling.

You can install the dependencies using pip:
pip install pandas numpy matplotlib seaborn scikit-learn

## How to Run

1.  **Clone the repository:**

2.  **Download the dataset:** Ensure the `Mall_Customers.csv` file is in the project directory.
3.  **Open the notebook:** Open the `customer_segmentation.ipynb` in a Jupyter environment (like Colab, Jupyter Notebook, or JupyterLab).
4.  **Run the cells:** Execute the cells sequentially to perform the analysis.

## Analysis Steps

1.  **Data Loading and Exploration:** Load the dataset and perform initial checks (head, info, shape, missing values, descriptive statistics).
2.  **Data Preprocessing:** Drop irrelevant columns (`CustomerID`) and prepare features for clustering.
3.  **Exploratory Data Analysis (EDA):** Visualize the distributions of features and relationships between key variables like 'Annual Income' and 'Spending Score'.
4.  **Feature Scaling:** Scale the selected features using `StandardScaler` as K-Means is sensitive to feature scales.
5.  **Elbow Method:** Use the Elbow Method to determine the optimal number of clusters (K) by plotting the Within-Cluster Sum of Squares (WCSS).
6.  **K-Means Clustering:** Apply the K-Means algorithm with the chosen optimal K to segment the customers.
7.  **Cluster Analysis and Visualization:** Add cluster labels to the dataset and visualize the clusters, often by plotting 'Annual Income' vs. 'Spending Score' with clusters colored differently and centroids marked. Analyze the characteristics of each cluster by examining the mean feature values within each group.

## Results

The analysis will produce:

- Plots showing the distributions of features.
- A scatter plot illustrating the relationship between 'Annual Income' and 'Spending Score'.
- An Elbow Method plot to help determine the optimal number of clusters.
- A scatter plot showing the customer segments based on the clustering results, with centroids marked.
- A table showing the mean feature values for each cluster, providing insights into the characteristics of each customer segment.

Based on the visualization and cluster analysis, you can interpret the characteristics of each customer segment (e.g., high-income/high-spending, low-income/low-spending, etc.).

## Contributing

Feel free to fork this repository and contribute by improving the analysis, adding more features, or trying different clustering techniques.
