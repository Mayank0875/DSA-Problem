## Title

Alex and the TNT

## Slug

alex-and-the-tnt

## Difficulty

Medium

## Description

Alex is participating in the filming of another video for BrMeast. BrMeast asked Alex to prepare 250 thousand tons of TNT, but Alex didn't hear him well, so he prepared $n$ boxes and arranged them in a row waiting for trucks. The $i$-th box from the left weighs $a_i$ tons.

All trucks that Alex is going to use hold the same number of boxes, denoted by $k$. Loading happens in the following way:
- The first $k$ boxes go to the first truck,
- The second $k$ boxes go to the second truck,
- ...
- The last $k$ boxes go to the $(n/k)$-th truck.

Upon loading is completed, each truck must have **exactly** $k$ boxes. In other words, if $n$ is not divisible by $k$, then the loading option with that $k$ is not possible.

Alex hates justice, so he wants the maximum absolute difference between the total weights of any two trucks to be as great as possible. If there is only one truck, this value is 0.

Alex has quite a lot of connections, so for every $1 \le k \le n$, he can find a company such that each of its trucks can hold exactly $k$ boxes. Your task is to print the maximum absolute difference between the total weights of any two trucks over all valid choices of $k$.

## Examples

### 1

#### Input

2
1 2

#### Output

1

#### Explanation

We can choose $k=1$. Truck 1 gets box 1 (weight 1), Truck 2 gets box 2 (weight 2). Difference is $|2-1| = 1$.
If we choose $k=2$, there is only one truck with weight $1+2=3$. Difference is 0.
Max difference is 1.
    
### 2

#### Input

4
1000000000 1000000000 1000000000 1000000000

#### Output

0

#### Explanation
All boxes are equal. Regardless of $k$, all trucks will have equal weight.


## Input Format  

- The first line contains one integer $n$ — the number of boxes.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the weights of the boxes.

## Output Format  

- Return a single integer — the maximum absolute difference.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ a[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, math, number-theory

## Company
tiktok