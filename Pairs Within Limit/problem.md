## Title

Pairs Within Limit

## Slug

pairs-within-limit

## Difficulty

Easy

## Description

You are given an array of integers representing weights and a maximum limit x.
You can form pairs such that the sum of the two numbers in each pair does not exceed x.
Each element can belong to at most one pair.

If an element cannot be paired, it can remain alone as a single element (which also counts as one group).

Your task is to determine the minimum number of groups (pairs or singles) required so that:
	•	The sum of elements in every group is ≤ x.

## Examples

### 1

#### Input

4 10 
[7, 2, 3, 9]

#### Output

3

#### Explanation

Possible grouping:
	(2, 7) → sum = 9 ≤ 10
	(3) → sum = 3 ≤ 10
	(9) → sum = 9 ≤ 10
Total groups = 3.
    
### 2

#### Input

5 5 
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

Possible grouping:
	(2, 3) → sum = 5 ≤ 5
	(2, 2) → sum = 4 ≤ 5
	(4) → sum = 4 ≤ 5
Total groups = 3.

## Input Format  

- The first line contains two integers n and x: the number of elements and the maximum allowed sum per group.
- The second line contains n integers a₁, a₂, ..., aₙ — the elements of the array.

## Output Format  

- Return a single integer: the minimum number of groups required.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ a_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers