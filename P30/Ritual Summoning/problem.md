## Title

Ritual Summoning

## Slug

ritual-summoning

## Difficulty

Easy

## Description

A summoning ritual requires exactly $T$ units of "life energy". You can make sacrifices of different types, each providing a set amount of energy (e.g., 2, 3, 5). You can perform an unlimited number of each sacrifice. Your task is to find the *total number* of unique combinations of sacrifices that will sum to $T$.

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