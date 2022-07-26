This project was based on Yelp Dataset and they were all implemented for large datasets by pyspark and efficient algorithms.

Dataset Overview:https://www.yelp.com/dataset/documentation/main

Because of privacy consideration and the requiement of our professor, all codes should not be uploaded on Github AND if you would like to have a look at my codes or  discuss with me about these algorithms, please contact me with email: hongyis@marshall.usc.edu and I will sent you a copy of my codes.

1. Association rules: Apriori + PCY optimization + SON algorithms
 -PCY: Create a bit-array to make full use of the ram in the first pass
 -SON: Avoids false negatives and false positives, requires two full passes over data

2. Recommendation System: Neighborhood-based/user-based/item-based collaborating filtering + Jaccard + Pearson Corr + memory-based
 -Jaccard/pearson Corr: A similarity measurement
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
