# -YouTube-Comment-Clustering

## Project Overview

This project focuses on clustering YouTube comments using machine learning techniques, specifically K-means and Hierarchical Clustering. The primary objective is to identify clusters of spam comments, enabling better content moderation and spam mitigation.

## Dataset

The dataset used in this project contains:

- 861,962 rows and 9 columns.

- Comments from videos of four YouTubers: Cleo Abram, Physics Girl, Jet Lag: The Game, and Neo.

- Key features include Comment (Actual) and Comment Author.

# Dataset Highlights:

- Large-scale data requiring preprocessing.

- Missing values managed by retaining non-null entries.

- Text data converted into numerical representations for clustering.

## Methodology

1. Data Preprocessing

  - Removed unnecessary HTML tags, punctuation marks, and NaN values.

  - Focused on relevant columns: Comment (Actual) and Comment Author.

2. Feature Engineering

  - Text to Numerical Conversion:

    - Used the Word2Vec model from the gensim library to vectorize comments.

    - Achieved a 100-dimensional vector representation for each comment.

  - Dimensionality Reduction:

    - Reduced vectors to a 1D array (using PCA) for clustering.

3. Clustering

  - K-means Clustering:

    - Performed clustering on the entire dataset.

    - Visualized clusters to identify patterns.

  - Hierarchical Clustering:

    - Applied on a sample of 1,000 points for computational feasibility.

## Tools and Technologies

- Programming Languages: Python

- Libraries: gensim for Word2Vec, numpy, pandas, matplotlib

## Results

- Successfully clustered comments into meaningful groups.

- Identified spam comment clusters for further analysis.


## Future Work

- Expand clustering methods to include DBSCAN or other density-based algorithms.

- Automate spam detection based on cluster properties.

- Integrate with a real-time comment moderation system.
