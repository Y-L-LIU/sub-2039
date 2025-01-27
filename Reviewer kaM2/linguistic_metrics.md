linguistic metrics 

 2.1 Readability
we choose Flesch Reading Ease (FSE) to measure the readability. The formula for calculating the FSE is as follows:
206.835 – 1.015 x (total words / total sentences) – 84.6 x (total syllables / total words)
The FSE ranges from 0 to 100. The higher the score, the easier it is for viewers to read.  We measure all the text in every domain and calculate the average score. The result is shown as below table:

| | Moonshot | gpt35  | Mixtral | Llama3 | gpt-4omini |
|---|----------|--------|---------|--------|------------|
| Physics_MGT |27.019| 27.825| 34.013 |30.627| 29.643     |
| Physics_HWT|37.458| 36.867 | 36.876  | 37.175 | 36.894  |
| Medicine_MGT|33.986|35.975 | 36.175  |32.26 |28.037     |
| Medicine_HWT               | 37.356   | 37.598 | 37.408  | 37.435 | 37.619     |
| Biology_MGT                | 26.514   | 31.56  | 31.437  | 26.877 | 25.124     |
| Biology_HWT                | 34.249   | 34.076 | 34.099  | 34.243 | 34.112     |
| Electrical_engineering_MGT | 28.851   | 33.889 | 31.982  | 26.66  | 27.067     |
| Electrical_engineering_HWT | 35.843   | 35.407 | 35.594  | 35.759 | 35.498     |
| Computer_science_MGT       | 26.802   | 33.468 | 32.186  | 28.172 | 27.167     |
| Computer_science_HWT       | 35.407   | 35.551 | 35.507  | 35.33  | 35.6       |
| Literature_MGT             | 50.8     | 47.893 | 54.321  | 57.056 | 43.76      |
| Literature_HWT             | 55.856   | 56.083 | 55.991  | 56.022 | 55.996     |
| History_MGT                | 53.612   | 49.885 | 56.435  | 60.663 | 48.998     |
| History_HWT                | 57.783   | 57.876 | 57.892  | 57.867 | 57.854     |
| Education_MGT              | 31.739   | 32.401 | 33.995  | 32.02  | 25.055     |
| Education_HWT              | 36.172   | 36.516 | 36.596  | 36.064 | 36.53      |
| Art_MGT                    | 48.835   | 47.196 | 52.74   | 56.135 | 42.901     |
| Art_HWT                    | 51.692   | 52.581 | 52.69   | 52.324 | 52.77      |
| Law_MGT                    | 39.413   | 39.278 | 42.736  | 44.188 | 33.608     |
| Law_HWT                    | 40.695   | 41.944 | 41.748  | 41.352 | 41.886     |
| Management_MGT             | 28.861   | 30.427 | 30.021  | 25.038 | 22.923     |
| Management_HWT             | 32.236   | 32.401 | 32.631  | 32.241 | 32.38      |
| Philosophy_MGT             | 36.482   | 36.539 | 40.951  | 40.324 | 30.34      |
| Philosophy_HWT             | 41.859   | 42.107 | 42.13   | 41.516 | 42.098     |
| Economy_MGT                | 28.517   | 34.289 | 33.085  | 28.577 | 28.122     |
| Economy_HWT                | 34.672   | 34.592 | 34.95   | 34.942 | 34.63      |
| Math_MGT                   | 32.218   | 37.836 | 39.132  | 34.738 | 37.189     |
| Math_HWT                   | 39.032   | 38.946 | 39.033  | 39.031 | 38.925     |
| Statistics_MGT             | 21.7     | 28.607 | 28.345  | 23.83  | 23.313     |
| Statistics_HWT             | 29.871   | 29.933 | 29.902  | 29.943 | 29.846     |
| Chemistry_MGT              | 35.248   | 37.823 | 36.633  | 31.127 | 30.111     |
| Chemistry_HWT              | 34.73    | 33.978 | 34.252  | 34.483 | 33.981     |

We find that the MGT’s FRE in almost all domins are higher that higher that HWT’s FRE.

2.2 Diversity
We choose Text-Token Ratio (TTR) to measure the diversity of text. It is defined as the ratio of unique tokens divided by the total number of tokens. This measurement is bounded between 0 and 1. If there is no repetition in the text this measurement is 1, and if there is infinite repetition, it will tend to 0.

We measure all the text in every domain and calculate the average score. The result is shown as below table:

|    | Moonshot | gpt35 | Mixtral | Llama3 | gpt-4omini |
|-----|----------|-------|---------|--------|------------|
| Physics_MGT  | 0.5 | 0.58  | 0.481 | 0.494 | 0.491      |
| Physics_HWT | 0.41 | 0.413 | 0.413| 0.411  | 0.413      |
| Medicine_MGT | 0.561    | 0.617 | 0.565   | 0.581  | 0.635      |
| Medicine_HWT               | 0.615    | 0.614 | 0.615   | 0.614  | 0.614      |
| Biology_MGT                | 0.533    | 0.582 | 0.523   | 0.544  | 0.567      |
| Biology_HWT                | 0.497    | 0.497 | 0.497   | 0.497  | 0.497      |
| Electrical_engineering_MGT | 0.523    | 0.566 | 0.503   | 0.534  | 0.561      |
| Electrical_engineering_HWT | 0.493    | 0.492 | 0.493   | 0.493  | 0.492      |
| Computer_science_MGT       | 0.52     | 0.563 | 0.493   | 0.527  | 0.547      |
| Computer_science_HWT       | 0.464    | 0.46  | 0.462   | 0.464  | 0.46       |
| Literature_MGT             | 0.546    | 0.65  | 0.552   | 0.526  | 0.618      |
| Literature_HWT             | 0.524    | 0.525 | 0.525   | 0.525  | 0.525      |
| History_MGT                | 0.52     | 0.626 | 0.527   | 0.499  | 0.549      |
| History_HWT                | 0.454    | 0.454 | 0.454   | 0.454  | 0.454      |
| Education_MGT              | 0.548    | 0.61  | 0.555   | 0.556  | 0.632      |
| Education_HWT              | 0.588    | 0.589 | 0.589   | 0.588  | 0.589      |
| Art_MGT                    | 0.547    | 0.635 | 0.547   | 0.526  | 0.61       |
| Art_HWT                    | 0.534    | 0.531 | 0.53    | 0.531  | 0.529      |
| Law_MGT                    | 0.53     | 0.613 | 0.53    | 0.536  | 0.612      |
| Law_HWT                    | 0.563    | 0.56  | 0.562   | 0.563  | 0.561      |
| Management_MGT             | 0.548    | 0.584 | 0.546   | 0.574  | 0.635      |
| Management_HWT             | 0.598    | 0.596 | 0.596   | 0.598  | 0.597      |
| Philosophy_MGT             | 0.537    | 0.644 | 0.541   | 0.524  | 0.626      |
| Philosophy_HWT             | 0.54     | 0.538 | 0.539   | 0.536  | 0.539      |
| Economy_MGT                | 0.53     | 0.587 | 0.517   | 0.524  | 0.586      |
| Economy_HWT                | 0.536    | 0.534 | 0.534   | 0.533  | 0.534      |
| Math_MGT                   | 0.485    | 0.542 | 0.467   | 0.468  | 0.508      |
| Math_HWT                   | 0.452    | 0.451 | 0.45    | 0.449  | 0.451      |
| Statistics_MGT             | 0.511    | 0.551 | 0.475   | 0.506  | 0.504      |
| Statistics_HWT             | 0.408    | 0.408 | 0.408   | 0.41   | 0.408      |
| Chemistry_MGT              | 0.539    | 0.589 | 0.536   | 0.605  | 0.632      |
| Chemistry_HWT              | 0.614    | 0.61  | 0.611   | 0.613  | 0.61       |


2.3 Syntactic complexity
2.3.1 ASL
We first choose Average Sentence Length (ASL) to measure the Syntactic complexity of text, which is the average number of words per sentence in a text,

We measure all the text in every domain and calculate the average score. The result is shown as below table:
|    | Moonshot | gpt35  | Mixtral | Llama3 | gpt-4omini |
|----|----------|--------|---------|--------|------------|
| Physics_MGT| 24.723 |22.999 |22.869|22.997 | 21.192 |
| Physics_HWT| 23.092 |23.098| 23.08| 23.085  | 23.1      |
| Medicine_MGT|21.094|21.081| 17.858| 21.683 | 21.379     |
| Medicine_HWT | 23.888| 23.461|23.658|23.829| 23.454     |
| Biology_MGT|22.596| 22.702 |20.151| 22.365 | 21.139     |
| Biology_HWT| 22.855|23.048| 23.023| 22.859 | 23.019     |
| Electrical_engineering_MGT | 22.403   | 21.923 | 20.515  | 21.669 | 20.806     |
| Electrical_engineering_HWT | 22.104   | 22.189 | 22.124  | 22.099 | 22.182     |
| Computer_science_MGT       | 22.738   | 22.32  | 20.928  | 21.495 | 20.414     |
| Computer_science_HWT       | 21.884   | 21.884 | 21.874  | 21.913 | 21.868     |
| Literature_MGT             | 21.247   | 20.881 | 17.821  | 19.545 | 21.559     |
| Literature_HWT             | 23.486   | 23.444 | 23.472  | 23.439 | 23.465     |
| History_MGT                | 21.176   | 21.624 | 18.998  | 19.19  | 21.02      |
| History_HWT                | 24.943   | 24.844 | 24.883  | 24.925 | 24.93      |
| Education_MGT              | 21.369   | 21.352 | 17.408  | 21.306 | 21.1       |
| Education_HWT              | 23.753   | 23.571 | 23.587  | 23.823 | 23.561     |
| Art_MGT                    | 21.28    | 21.217 | 18.276  | 19.593 | 21.436     |
| Art_HWT                    | 24.902   | 24.805 | 24.812  | 24.89  | 24.747     |
| Law_MGT                    | 21.917   | 21.893 | 19.036  | 21.127 | 21.92      |
| Law_HWT                    | 25.749   | 25.246 | 25.39   | 25.515 | 25.255     |
| Management_MGT             | 21.224   | 21.562 | 17.817  | 22.163 | 20.897     |
| Management_HWT             | 23.886   | 23.665 | 23.656  | 23.838 | 23.654     |
| Philosophy_MGT             | 22.057   | 21.215 | 18.189  | 20.912 | 21.506     |
| Philosophy_HWT             | 24.949   | 24.801 | 24.735  | 25.084 | 24.752     |
| Economy_MGT                | 22.943   | 22.106 | 20.08   | 21.816 | 20.926     |
| Economy_HWT                | 23.82    | 23.966 | 23.836  | 23.801 | 23.974     |
| Math_MGT                   | 23.463   | 21.738 | 21.331  | 21.39  | 16.913     |
| Math_HWT                   | 20.487   | 20.366 | 20.382  | 20.151 | 20.368     |
| Statistics_MGT             | 24.039   | 23.369 | 22.258  | 21.427 | 19.855     |
| Statistics_HWT             | 21.489   | 21.735 | 21.751  | 21.612 | 21.73      |
| Chemistry_MGT              | 20.342   | 19.632 | 16.764  | 21.451 | 20.105     |
| Chemistry_HWT              | 22.26    | 22.62  | 22.443  | 22.169 | 22.672     |

2.3.2 SCI
We then choose Sentence Complexity Index (SCI) to measure the Syntactic complexity of text, which analyze the number and types of syntactic components it contains, such as subordinate clauses, coordinate clauses, and other grammatical structures.
We measure all the text in every domain and calculate the average score. The result is shown as below table:
|                            | Moonshot | gpt35   | Mixtral | Llama3  | gpt-4omini |
|----------------------------|----------|---------|---------|---------|------------|
| Physics_MGT                | 25.376   | 16.243  | 26.5    | 22.156  | 40.515     |
| Physics_HWT                | 59.99    | 58.788  | 58.742  | 59.264  | 58.674     |
| Medicine_MGT               | 23.832   | 17.909  | 23.196  | 18.458  | 15.347     |
| Medicine_HWT               | 15.773   | 15.744  | 15.783  | 15.735  | 15.761     |
| Biology_MGT                | 25.879   | 20.106  | 26.675  | 21.298  | 30.805     |
| Biology_HWT                | 47.198   | 47.254  | 47.337  | 47.217  | 47.283     |
| Electrical_engineering_MGT | 25.584   | 20.061  | 26.727  | 21.161  | 26.906     |
| Electrical_engineering_HWT | 41.753   | 41.63   | 41.542  | 41.736  | 41.574     |
| Computer_science_MGT       | 27.045   | 20.996  | 28.614  | 21.893  | 31.894     |
| Computer_science_HWT       | 52.757   | 54.108  | 53.881  | 53.132  | 54.243     |
| Literature_MGT             | 43.958   | 17.387  | 37.767  | 49.288  | 38.817     |
| Literature_HWT             | 77.576   | 76.314  | 76.183  | 76.222  | 76.122     |
| History_MGT                | 57.165   | 22.651  | 46.698  | 60.834  | 68.094     |
| History_HWT                | 114.21   | 113.829 | 113.97  | 113.883 | 113.867    |
| Education_MGT              | 28.366   | 19.479  | 26.821  | 28.308  | 18.344     |
| Education_HWT              | 25.289   | 25.089  | 25.008  | 25.112  | 25.043     |
| Art_MGT                    | 40.091   | 18.139  | 36.549  | 47.711  | 36.369     |
| Art_HWT                    | 65.562   | 67.752  | 68.19   | 67.551  | 68.468     |
| Law_MGT                    | 30.046   | 17.391  | 29.164  | 32.717  | 21.047     |
| Law_HWT                    | 31.597   | 33.138  | 32.763  | 31.695  | 33.243     |
| Management_MGT             | 25.637   | 21.895  | 25.766  | 19.597  | 15.422     |
| Management_HWT             | 16.286   | 16.244  | 16.274  | 16.122  | 16.231     |
| Philosophy_MGT             | 36.931   | 17.369  | 33.692  | 40.009  | 26.797     |
| Philosophy_HWT             | 60.751   | 60.206  | 59.507  | 62.056  | 59.528     |
| Economy_MGT                | 26.126   | 19.193  | 26.788  | 22.587  | 23.937     |
| Economy_HWT                | 32.723   | 33.417  | 33.744  | 33.565  | 33.323     |
| Math_MGT                   | 26.143   | 21.403  | 25.957  | 22.76   | 32.815     |
| Math_HWT                   | 41.403   | 41.549  | 41.633  | 41.808  | 41.619     |
| Statistics_MGT             | 27.556   | 21.56   | 29.854  | 23.123  | 42.011     |
| Statistics_HWT             | 68.066   | 68.24   | 68.19   | 67.673  | 68.181     |
| Chemistry_MGT              | 21.966   | 18.26   | 21.362  | 10.836  | 13.9       |
| Chemistry_HWT              | 13.104   | 13.128  | 13.174  | 13.061  | 13.197     |
