## Title

Restaurant Menu Combos

## Slug

restaurant-menu-combos

## Difficulty

Medium

## Description

A restaurant's menu has $N$ items. You are given a list of $N$ specific dishes that a table ordered, with prices $candidates_i$. The list may include duplicates (e.g., two people ordered the 'pasta' for 5). You want to find a subset of these *specific* dishes that adds up to a target price $T$ (e.g., to split the bill). Your task is to find the *total count* of unique combinations of these dishes that sum to $T$. Each dish from the list may be used *only once*.

## Examples

### 1

#### Input

7 8 
[10, 1, 2, 7, 6, 1, 5]

#### Output

4

#### Explanation

The 4 unique combinations are [1, 1, 6], [1, 2, 5], [1, 7], and [2, 6].    

### 2

#### Input

5 5 
[2, 5, 2, 1, 2]

#### Output

2

#### Explanation
The 2 unique combinations are [1, 2, 2] and [5].

## Input Format  

- The first line contains two integers, $N$ and $T$, representing the number of candidate numbers and the target sum.
- The second line contains $N$ space-separated integers, $candidates_i$.

## Output Format  

- Return single integer representing the total number of unique combinations that sum to the target.
  

## Constraints  

- 1 ≤ n ≤ 100
- 1 ≤ candidates[i] ≤ 50
- 1 ≤ target ≤ 30

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion