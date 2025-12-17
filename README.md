Customer Segmentation - Unsupervised Learning Project

📌 Project Overview
This project performs Customer Segmentation using unsupervised learning techniques on a marketing campaign dataset. The goal is to identify distinct customer "personas" based on demographics, purchasing behavior, and household structure. These clusters enable businesses to tailor marketing strategies, optimize product offerings, and improve customer retention.

🛠️ Technologies & Libraries
The project is implemented in Python using the following libraries:

Data Manipulation: pandas, numpy

Visualization: matplotlib, seaborn, yellowbrick

Machine Learning: scikit-learn (KMeans, AgglomerativeClustering, PCA, StandardScaler)

📂 Dataset & Features
The analysis uses a dataset containing customer demographics, purchasing history, and campaign responses.

Feature Engineering

To improve clustering performance, several new features were engineered:

Age: Calculated from birth year.

Spent: Total amount spent across all categories (Wines, Fruits, Meat, Fish, Sweets, Gold).

Living_With: Simplified marital status into "Partner" or "Alone".

Children: Total count of children (Kidhome + Teenhome) in the household.

Family_Size: Total members in the household.

Is_Parent: Binary flag indicating parenthood.

Education: Segmented into Undergraduate, Graduate, and Postgraduate.

⚙️ Methodology
Data Cleaning: Handling missing values and converting date formats.

Preprocessing: Categorical encoding and standard scaling of data.

Dimensionality Reduction: Using Principal Component Analysis (PCA) to reduce the dataset to 3 components for better visualization and noise reduction.

Clustering:

Used the Elbow Method to determine the optimal number of clusters.

Applied Agglomerative Clustering to segment customers.

Evaluation: Visualized clusters in 3D space and profiled them based on statistical means.

📊 Results: Customer Clusters
The analysis identified 4 distinct customer clusters, each requiring a unique marketing strategy:

Cluster 0: The "Standard Family"

Profile: Definitely parents, typically with 2-4 household members. Most have a teenager at home and are relatively older.

Strategy: Focus on convenience and family value. Offer multi-buy discounts (e.g., "Buy 2 Get 1 Free"), family-sized meal kits, and traditional marketing (flyers).

Cluster 1: The "New Parents"

Profile: Younger customers, majority are parents with exactly one young child (no teenagers). Small families (max 3 members).

Strategy: Focus on child-centric and healthy products. Promote organic baby food, run social media campaigns, and offer personalized coupons via apps.

Cluster 2: The "Elite Spenders"

Profile: High-income group, spanning all ages. Definitely not parents. Max 2 members (couples or singles).

Strategy: Focus on luxury and quality. Promote premium wines, imported meats, and gourmet products. Use elegant email newsletters and exclusive event invitations.

Cluster 3: The "Budget-Conscious Family"

Profile: Lower-income group, relatively older. Large families (up to 5 members), typically with teenagers.

Strategy: Focus on savings and bulk buying. Promote store-brand products, weekly sales circulars, and loyalty programs that offer cash-back rewards.
