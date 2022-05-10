This project contains codes for many algorithms. They are all implemented for large datasets by pyspark and more efficient methods:

For privacy consideration, all codes are not uploaded on Github AND if you would like to talk about these algorithms below with me, please contact me with email: hongyi.shao.2022@marshall.usc.edu

1. Association rules: Apriori + PCY optimization + SON algorithms
 -PCY: Create a bit-array to make full use of the ram in the first pass
 -SON: Avoids false negatives and false positives, requires two full passes over data

2. Recommendation System: Neighborhood-based/user-based/item-based collaborating filtering + Jaccard + Pearson Corr + memory-based
 -Jaccard/pearson Corr: A similarity measure
 -Memory-based: Case Amplification

3. Community/Social Network Detection: Girvan-Newman Algorithm + Modularity Evaluation + Hierarchical Decomposition
 -Girvan-Newman Algorithm: Start with one cluster and recursively split it based on the betweenness value
 -Betweenness: Number of shortest paths passing through the edge
 -Modularity Evaluation: Evaluation metric to decide the best cut

4. Stream Analysis: Fixed-size (reservoir) sampling; Bloom filter
 -Fixed-size (reservoir) sampling: Store all the first s elements, for n > s, keep or discard with probability calculated
 -Bloom filter: No false negatives

5. Clustering Analysis: Bradley-Fayyad-Reina
 -Bradley-Fayyad-Reina: for uniform-distributed axis-aligned shapes, DS, CS, RS
