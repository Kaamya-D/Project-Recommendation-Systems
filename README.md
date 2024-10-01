# Project-Recommendation_Systems
**A study on the Channel Coding Perspective of Recommendation Systems**
![image](https://github.com/user-attachments/assets/7a961187-942f-411b-87e1-aece7db99c27)
The paper an innovative approach to solving recommendation system problems by using concepts from information theory, particularly channel coding. Traditional recommendation systems predict user ratings for items based on observed data, typically with the assumption that missing entries need to be completed (e.g., Netflix Prize). However, this project assumes the ratings matrix has a block-constant structure, where both users and items are clustered, and ratings are corrupted by erasures and errors. The goal is to analyze how well this underlying rating matrix can be recovered from sparse, noisy observations.

The project introduces a coding-theoretic perspective where the aim is not to complete the matrix but to recover the underlying block-constant matrix from the noisy observations.

![image](https://github.com/user-attachments/assets/37dd24cf-ebe2-4b29-a078-0d31c85d2775)

The paper explores the recovery of a binary matrix representing user-item ratings, where matrix entries are first permuted and then corrupted by erasure and error channels. The matrix is assumed to have block-constant structure, meaning groups of similar users rate similar items the same.
![image](https://github.com/user-attachments/assets/b70916a2-bcee-45b1-96da-33e9c0b01ea1)
![image](https://github.com/user-attachments/assets/15a57664-b8b6-4d2b-b189-2c838df58fc0)

**Model:** The matrix's rows and columns are permuted, followed by transmission through erasure and binary symmetric channels (BSC), which introduce noise and missing entries, respectively.

**Bounds:** The project establishes upper and lower bounds for the probability of error in recovering the original matrix. It shows that recovery becomes possible if the cluster sizes exceed a threshold proportional to the logarithm of the matrix dimensions.

**Algorithms:** An algorithm has been proposed for clustering rows and columns, followed by estimating cluster values. The paper provides conditions under which the probability of error diminishes to zero as the matrix size increases. It also uses-  Probability of Error When Clustering is Known, Probability of Error in Clustering and Estimation Under Unknown Clustering
![image](https://github.com/user-attachments/assets/af057e1c-89fd-4c3e-b180-35d4c8a872fc)

**Conclusion-**
This project successfully bridges the gap between recommendation systems and channel coding theory, offering insights into how clusters of users and items can be accurately recovered despite noisy and missing data. We considered the problem of estimating a block constant rating matrix. The observed matrix is obtained through unknown relabeling of the rows and columns of the underlying matrix, followed by an error and erasure channel. Our probability of error analysis showed that if the number of row clusters and the number column clusters are Ω(ln(m)) and Ω(ln(n)) respectively, then the matrix can be clustered and estimated with vanishing probability of error if the cluster sizes are Ω(ln(mn)).


