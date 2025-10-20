## Title

Distributing Ancient Scrolls

## Slug

distributing-ancient-scrolls

## Difficulty

Medium

## Description

A wise librarian must distribute n ancient scrolls, arranged sequentially on a shelf, among k waiting scribes. Each scroll i has x[i] pages, representing the effort needed to copy it. 
The scrolls must be assigned to scribes in contiguous blocks as they appear on the shelf (e.g., scribe 1 gets scrolls 1 to j, scribe 2 gets scrolls j+1 to m, etc.). 
To ensure fairness, the librarian wants to minimize the workload of the busiest scribe. Find the minimum possible value for the maximum number of pages assigned to any single scribe.


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

- The first line contains two integers n and k: the number of scrolls and the number of scribes.
- The second line contains n integers x[1], x[2] ... x[n] , where x[i] is the time in seconds it takes for the i-th machine to produce one toy.

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
