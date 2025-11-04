## Title

Fair Allotment of Land

## Slug

fair-allotment-of-land

## Difficulty

Medium

## Description

A kingdom has `n` plots of land for sale, arranged in a line along a river. Plot `i` has a value of `x[i]`. The king wants to sell these plots to `k` barons. Each baron must purchase a contiguous block of one or more plots. To prevent any one baron from becoming too powerful, the king wants to minimize the maximum total value of land any single baron can acquire. Find this minimum-maximum value.

## Examples

### 1

#### Input

5 3 
2 4 7 3 5


#### Output

8

#### Explanation

An optimal distribution assigns scrolls [2, 4] to the first scribe (sum 6 pages), scroll [7] to the second scribe (sum 7 pages), and scrolls [3, 5] to the third scribe (sum 8 pages). The maximum number of pages assigned to any scribe is 8. No other distribution into 3 contiguous blocks can achieve a maximum load less than 8.

### 2

#### Input

1 1
34

#### Output

34


#### Explanation

No other distribution into 1 contiguous blocks can achieve a maximum load less than 34.

## Input Format

- The first line contains two integers `n` and `k`: the number of plots and the number of barons.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the value of the i-th plot.

## Output Format

- Return one integer: the minimum possible value for the maximum number of pages assigned to any scribe.

## Constraints

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy