## Title

Manufacturing Anomaly

## Slug

manufacturing-anomaly

## Difficulty

Medium

## Description

A factory's assembly line produces components, sorted by serial number. For quality control, every component is duplicated, so each serial number should appear twice in a row. A glitch has caused one component to not be duplicated. Given the sorted list of serial numbers, find the serial number of the single, non-duplicated component.

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

- The first line contains an odd integer n, the total number of components.
- The second line contains n space-separated integers representing the sorted serial numbers.

## Output Format

- Return a single integer: the serial number of the component that appears only once.

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