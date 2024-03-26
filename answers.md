# CMPS 2200 Reciation 5
## Answers

**Name:** Julia Renner


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.** How do the running times compare to the asymptotic bounds? How does changing the type of input list change the relative performance of these algorithms?

The running times of the quicksort algorithms do not strictly abide by their asymptotic bounds, especially for larger input sizes. Changing the type of input list from random to sorted slowed both the fixed-pivot and random-pivot algorithms, however tim-sort maintained much more consistent speed across both differing sizes and types of input lists. 

Random:
|      n |   qsort-fixed-pivot |   qsort-random-pivot |   tim-sort |
|--------|---------------------|----------------------|------------|
|    100 |               0.228 |                0.386 |      0.013 |
|    200 |              43.793 |                1.058 |      0.034 |
|    500 |               1.506 |                1.851 |      0.061 |
|   1000 |               2.741 |                6.541 |      0.146 |
|   2000 |               7.552 |                8.729 |      0.442 |
|   5000 |              69.320 |               28.715 |      1.287 |
|  10000 |             108.207 |              112.087 |      2.205 |
|  20000 |             301.756 |              217.723 |      5.311 |
|  50000 |             803.573 |              615.961 |     12.812 |
| 100000 |            1293.917 |             1595.177 |     86.292 |

Sorted:
|      n |   qsort-fixed-pivot |   qsort-random-pivot |   tim-sort |
|--------|---------------------|----------------------|------------|
| 100000 |            1453.717 |             1873.680 |     96.373 |
|  50000 |             610.643 |              676.820 |     15.231 |
|  20000 |             217.592 |              281.698 |      7.339 |
|  10000 |             104.038 |              116.765 |     50.615 |
|   5000 |              25.282 |               91.058 |      0.802 |
|   2000 |               7.030 |               23.375 |      0.378 |
|   1000 |              15.854 |               26.607 |      0.129 |
|    500 |               1.254 |                1.759 |      0.061 |
|    200 |               0.425 |                0.543 |      0.021 |
|    100 |               0.198 |                0.267 |      0.009 |


- **1c.**

|      n |   qsort-fixed-pivot |   qsort-random-pivot |   tim-sort |
|--------|---------------------|----------------------|------------|
|    100 |               0.212 |                0.267 |      0.014 |
|    200 |               0.830 |                0.612 |      0.024 |
|    500 |               1.384 |                1.438 |      0.065 |
|   1000 |               2.611 |                3.532 |      0.136 |
|   2000 |               5.961 |               71.517 |      0.510 |
|   5000 |              17.618 |               19.691 |      0.796 |
|  10000 |             117.775 |               99.843 |      1.842 |
|  20000 |             178.964 |              210.060 |      4.031 |
|  50000 |             576.812 |              648.967 |     58.526 |
| 100000 |            1280.373 |             1804.602 |     99.124 |