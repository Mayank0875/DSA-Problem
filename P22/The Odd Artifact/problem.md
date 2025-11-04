## Title

The Odd Artifact

## Slug

the-odd-artifact

## Difficulty

Medium

## Description

An archaeologist has found `n` artifacts, sorted by their excavation date. The museum's cataloging system requires artifacts to be entered in pairs (e.g., a pot and its lid). Every artifact in the list has a matching pair and appears twice in a row, except for one unique item. Find the date of this single, unpaired artifact.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of artifacts.
- The second line contains n space-separated integers representing the sorted excavation dates.

## Output Format

- Return a single integer: the date of the artifact that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array