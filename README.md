# PCA on the Wisconsin breast cancer dataset

In this project, the Wisconsin breast cancer dataset is visualized in two dimensions using Principal Component Analysis (PCA). The process involves the following steps:

1. **Rescaling the Data:**
   - Utilize `sklearn.preprocessing.StandardScaler` to rescale the data, ensuring that every feature has a mean of 0 and a standard deviation of 1 across the various points in the dataset.

2. **Compute Top Two Principal Components:**
   - Use two different approaches:
      - **Direct SVD (Singular Value Decomposition):**
         - Compute the top two principal components directly using SVD without using any PCA built-ins.
      - **PCA from sklearn.decomposition:**
         - Use `sklearn.decomposition.PCA` to compute the top two principal components.

3. **Coordinate Calculation:**
   - For every data point, compute its coordinates (projections) along the two principal components.

4. **Scatterplot Visualization:**
   - Create a scatterplot of the dataset in 2 dimensions.
   - X-axis represents the first principal component, and the Y-axis represents the second.
   - Color the points based on their diagnosis (malignant or benign).

The two approaches (direct SVD and PCA from sklearn.decomposition) should yield exactly the same results, with potential sign differences that can be resolved by flipping signs to ensure identical representations. The scatterplots generated for both approaches should be identical. The analysis aims to explore whether the data is roughly separable in two dimensions, providing insights into the inherent structure of the dataset.
