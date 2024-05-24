# RS-Algorithm-Performance-Code

This repository contains the code on Recommender System Report.

## Data

The data used in this project is the MovieLens 1M dataset. 
The dataset can be downloaded from the following link: https://grouplens.org/datasets/movielens/1M/

## Code

4 different algorithms is implemented in this report.

In Matrix Factorization and Factorization Machine, the code is runned in Kaggle Notebook environment,
which has Linux environment, Intel(R) Xeon(R) CPU @ 2.20GHz, 32GB RAM.

In GC-MC and IGMC, the code is runned in Docker container, 
which has Linux environment on macOS, Apple M1 Pro CPU @ 3.23GHz, 32GB RAM.

## Results

The results of the algorithms are as follows:

| Model     | RMSE  |
|-----------|-------|
| MF (K=3)  | 1.063 |
| MF (K=5)  | 1.059 |
| MF (K=10) | 1.055 |
| FM (K=2)  | 0.850 |
| FM (K=3)  | 0.844 |
| FM (K=5)  | 0.839 |
| GC-MC     | 0.889 |
| IGMC      | 0.861 |

One can find results for FM and MF in the Jupyter Notebook cell output, 
and for GC-MC and IGMC in the result.jpeg in the respective directories.

## References

Matrix Factorization: [Paper](https://ieeexplore.ieee.org/document/5197422), [Code](https://www.kaggle.com/code/phamdinhkhanh/matrix-factorization-movie-length-1m/notebook)

Factorization Machine: [Paper](https://ieeexplore.ieee.org/document/5694074), [Code](https://github.com/floraxhuang/Movie-Recommendation-System.git)

Graph Convolutional Matrix Completion: [Page](https://arxiv.org/abs/1706.02263), [Code](https://github.com/riannevdberg/gc-mc.git)

Inductive Graph Convolutional Matrix Completion: [Page](https://arxiv.org/abs/1904.12058), [Code](https://github.com/muhanzhang/IGMC.git)