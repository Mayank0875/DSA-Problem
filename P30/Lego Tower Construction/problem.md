## Title

Lego Tower Construction

## Slug

lego-tower-construction

## Difficulty

Easy

## Description

You are building a Lego tower that must be exactly $T$ units tall. You have an infinite supply of bricks of different heights (e.g., 2, 3, 5 units). Your task is to find the *total number* of unique combinations of these bricks that can be stacked to reach the target height $T$. The order of bricks doesn't matter, only the count of each type.

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