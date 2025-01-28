# Exploring Clustering with K-Means and Expectation-Maximization (EM)
This Assignment is a part of our coursework which focuses on experimenting with two clustering techniques, K-Means and Expectation-Maximization (EM), to understand their advantages and disadvantages. The goal is to evaluate the quality of clustering using two metrics: accuracy and the Adjusted Rand Index (ARI). Additionally, the project explores the relationship between clustering performance and the KL divergence between data distributions.

Part A: Clustering with Varying Data Separation
Dataset Generation:
We generate synthetic datasets where one part of the data is distributed normally around the origin, and the other part is shifted along the x-axis by a varying amount. This shift helps analyze how data separation impacts clustering performance.

Clustering Analysis:
For each dataset, we apply both K-Means and EM clustering methods across 10 random initializations (runs). Visualizations are created to compare the clustering results for both methods on one example dataset.

Performance Evaluation:

Accuracy: The accuracy of clustering is computed by aligning cluster labels to the true labels for the best match.
Adjusted Rand Index (ARI): This measures the agreement between true labels and predicted clusters.
Both metrics are plotted against the level of data separation to understand how K-Means and EM perform under different conditions.
Visual Representation:

Accuracy vs. Data Separation: Separate dots are plotted for each run, using different colors to represent K-Means and EM.
ARI vs. Data Separation: Similar dots are plotted for ARI, highlighting differences between the two methods.
Part B: Clustering with Rotated Covariance Structures
Random Rotation and Covariance:
A random rotation matrix is generated to create datasets with varying covariance structures. These datasets include two clusters: one around the origin and another shifted along the x-axis.

KL Divergence:
The KL divergence between the two cluster distributions is computed to quantify the difference between their shapes and spread.

Clustering Methods:

K-Means with isotropic covariance (no covariance modeling).
K-Means with full covariance (considering cluster shapes).
EM clustering, which accounts for full covariance.
Each method is evaluated across 10 runs.
Performance Evaluation:
For each run, the accuracy and ARI of the three methods are computed and analyzed.

Visualization:

Accuracy vs. KL Divergence: Dots are plotted for all runs, with different colors representing the three methods.
ARI vs. KL Divergence: Similar plots are created for ARI to compare the clustering methods.
Tabular Results:
A table is included summarizing the results for all 10 runs, showing the accuracy, ARI, and KL divergence for each method.
