# Model Selection for Clustering Colorectal Cancer Data

Conducted a comparative analysis of K-means and Hierarchical clustering techniques to evaluate their performance on colorectal tissue data, utilizing two feature sets: PathologyGAN (PGE) and ResNet50.

Aimed to determine the most effective clustering approach by assessing the quality of clusters using V-measure and Silhouette scores.

Processed 5,000 colorectal tissue patches, categorizing them into 9 tissue types: Adipose (ADI), Background (BACK), Debris (DEB), Lymphocytes (LYM), Mucus (MUC), Smooth muscle (MUS), Normal colon mucosa (NORM), Cancer-associated stroma (STR), and Colorectal adenocarcinoma epithelium (TUM).

Applied PCA and UMAP techniques to reduce the dimensionality of the data while preserving key features. PCA transforms correlated variables into uncorrelated ones, while UMAP preserves global structure and offers superior run-time performance.

K-means Clustering: Determined optimal K values using the elbow method, conducting 75 iterations. Achieved highest accuracy of 71% for V-measure on UMAP data.

Hierarchical Clustering: Employed agglomerative approach with single and ward linkage methods. For single linkage, achieved a highest accuracy of 66.62% for ResNet50 UMAP data.

Utilized V-measure and Silhouette scores to evaluate cluster quality. V-measure combines homogeneity and completeness, while Silhouette scores range from -1 to 1, indicating the separation quality of clusters.

K-means Performance: Highest accuracy of 71% (V-measure-UMAP) and 62% (Silhouette-UMAP) for PathologyGAN.

Hierarchical Clustering Performance: For ward linkage, achieved 72.91% accuracy (V-measure-UMAP) for ResNet50 and 61.54% (Silhouette-UMAP) for PathologyGAN.
Visualized clustering results using multiple graphs for each technique and data set.
