## Title

Unmatched Log Entry

## Slug

unmatched-log-entry

## Difficulty

Medium

## Description

A security system logs every entry and exit with a user ID. In a sorted log, every ID should appear exactly twice (once for entry, once for exit), side-by-side. Due to a system glitch, one user's action was recorded only once. Given this sorted list of IDs, you must find the ID of the user with the single, unmatched log entry.

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

- The first line contains an odd integer n, the total number of log entries.
- The second line contains n space-separated integers representing the sorted user IDs.

## Output Format

- Return a single integer: the user ID that appears only once.

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