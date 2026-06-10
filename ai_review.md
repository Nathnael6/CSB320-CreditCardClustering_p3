# AI Review

Prompt used:

"I have written this analysis in this ipynb file for an assignment and am required to get feedback on it. Please provide this."

## AI Feedback

The analysis follows a clear clustering pipeline with data loading, cleaning, outlier removal, feature scaling, K-Means clustering, Hierarchical Clustering, and model evaluation. The use of StandardScaler is appropriate because the numerical features are on different scales, especially in the credit card dataset where average credit limit is much larger than the visit and call counts.

The notebook correctly uses the Elbow Method, silhouette score, and Davies-Bouldin score to compare cluster quality. For the credit card dataset, selecting 2 clusters is well supported because it produced the strongest silhouette score and lowest Davies-Bouldin score. For the mall customers dataset, choosing 5 clusters is reasonable because it balances interpretability with the elbow graph, even though the evaluation metrics continued improving for higher k values.

One  improvement would be to avoid adding cluster label columns directly into the scaled feature dataframe before all evaluations are complete. The notebook handles this correctly by dropping cluster label columns before evaluating Hierarchical Clustering, but separating feature data from labeled output data could make the workflow cleaner. Another improvement would be adding a dendrogram for the Hierarchical Clustering section to better explain how clusters merge at different distances.

Overall, the project demonstrates a solid understanding of unsupervised learning, clustering evaluation, and customer segmentation. The visualizations support the analysis, and the discussion explains the cluster results in a way that connects the technical output to real customer behavior.

## Reflection

The feedback made sense to me because it pointed out both strengths and possible improvements. I agree that separating the scaled features from the cluster-label dataframe would make the workflow cleaner. The dendrogram suggestion also stood out because it would make the Hierarchical Clustering section easier to understand visually.