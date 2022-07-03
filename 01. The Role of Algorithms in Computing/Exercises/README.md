
# Chapter 1. Exercises
## Algorithms
### 1.1-1
- Sorting: Obtaining the most purchased product within a time period.
- Convex Hull: Nuclear leak evacuation.
### 1.1-2
- Storage and Power Consumption.
### 1.1-3
- LinkedList:
	- Pros: Insertion and Deletion.
	- Cons: Random Access.
### 1.1-4
- Similar: finding path with shortest distance. Both need the minimal cost.
- Different: traveling-salesman has more constraints. Shortest path needs the minimal cost between two end-points while tsp needs the minimal cost while covering all the nodes.
### 1.1-5
- Best: Sort array of integres.
- Approximately: find the solution of differential equations.
## Algorithms as Technology
### 1.2-1
- Google maps.
- Streaming services recommendation systems
### 1.2-2
$8n^2 < 64n * lgn$
$2^n < n^8$
$2 \le n \le 43$
### 1.2-3
$100n^2 < 2^n$
$n \ge 15$
## Problems
### 1-1. Comparison of running time
$$
\begin{array}{cccccccc}
         & \text{1 second}  & \text{1 minute}    & \text{1 hour}       & \text{1 day}            & \text{1 month}          & \text{1 year}           & \text{1 century} \\\\
\hline
\lg n    & 2^{10^6}         & 2^{6 \times 10^7}  & 2^{3.6 \times 10^9} & 2^{8.64 \times 10^{10}} & 2^{2.59 \times 10^{12}} & 2^{3.15 \times 10^{13}} & 2^{3.15 \times 10^{15}} \\\\
\sqrt n  & 10^{12}          & 3.6 \times 10^{15} & 1.3 \times 10^{19}  & 7.46 \times 10^{21}     & 6.72 \times 10^{24}     & 9.95 \times 10^{26}     & 9.95 \times 10^{30} \\\\
n        & 10^6             & 6 \times 10^7      & 3.6 \times 10^9     & 8.64 \times 10^{10}     & 2.59 \times 10^{12}     & 3.15 \times 10^{13}     & 3.15 \times 10^{15} \\\\
n\lg n   & 6.24 \times 10^4 & 2.8 \times 10^6    & 1.33 \times 10^8    & 2.76 \times 10^9        & 7.19 \times 10^{10}     & 7.98 \times 10^{11}     & 6.86 \times 10^{13} \\\\
n^2      & 1000             & 7745               & 60000               & 293938                  & 1609968                 & 5615692                 & 56156922 \\\\
n^3      & 100              & 391                & 1532                & 4420                    & 13736                   & 31593                   & 146645 \\\\
2^n      & 19               & 25                 & 31                  & 36                      & 41                      & 44                      & 51 \\\\
n!       & 9                & 11                 & 12                  & 13                      & 15                      & 16                      & 17
\end{array}
$$

