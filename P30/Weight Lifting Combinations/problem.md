## Title

Weight Lifting Combinations

## Slug

weight-lifting-combinations

## Difficulty

Easy

## Description

You are a weightlifter trying to load a barbell to an exact weight of $T$. You have a set of weight plates of different sizes (e.g., 2, 3, 5). Your task is to find the *total number* of unique combinations of these plates that sum exactly to the target weight $T$. You have an unlimited supply of each plate type. (Note: The two sides of the barbell are combined, just find the total sum).

## Examples

### 1

#### Input

4 7 
[2, 3, 6, 7]

#### Output

2

#### Explanation

The two unique combinations are [2, 2, 3] and [7].

### 2

#### Input

3 8 
[2, 3, 5]

#### Output

3

#### Explanation

The three unique combinations are [2, 2, 2, 2], [2, 3, 3], and [3, 5].

## Input Format  

- The first line contains two integers, $N$ and $T$, representing the number of coin denominations and the target sum
- The second line contains $N$ distinct space-separated integers, $candidates_i$, representing the coin denominations.

## Output Format  

- Return single integer representing the total number of unique combinations that sum to the target.
  

## Constraints  

- 1 ≤ n ≤ 30
- 1 ≤ candidates[i] ≤ 40
- 1 ≤ target ≤ 40
- All elements of candidates are distinct.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion