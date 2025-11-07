## Title

Starlight Constellations

## Slug

starlight-constellations

## Difficulty

Medium

## Description

An astronomer is analyzing $N$ stars, each with a specific brightness value. They are looking for "perfect constellations," which are sets of four `distinct` stars (i.e., using four different indices) whose brightness values sum up to a specific `target` value. Your task is to count how many `unique` combinations of brightness values form a perfect constellation. For example, if two different sets of four stars both have brightness `[-1, 0, 0, 1]`, this combination is only counted once.

## Examples

### 1

#### Input

6 0
[1, 0, -1, 0, -2, 2]

#### Output

3

#### Explanation

The three unique combinations that sum to 0 are: `[-2, -1, 1, 2]`, `[-2, 0, 0, 2]`, and `[-1, 0, 0, 1]`.
    
### 2

#### Input

5 8 
[2, 2, 2, 2, 2]

#### Output

1

#### Explanation

There is only one unique combination that sums to 8: `[2, 2, 2, 2]`.  

## Input Format  

- The first line contains a single integer N, the number of stars.
- The second line contains a single integer target, the target brightness.
- The third line contains N space-separated integers, nums_i, representing the brightness of each star.

## Output Format  

- Return single integer representing the total count of unique quadruplets that sum to the target.
  

## Constraints  

- 1 ≤ x ≤ 100
- -1e9 ≤ target ≤ 1e9
- -1e9 ≤ nums[i] ≤ 1e9


## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, sorting, two-pointers