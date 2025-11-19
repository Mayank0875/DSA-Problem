## Title
Planetary Crater Ice

## Slug
planetary-crater-ice

## Difficulty
Medium

## Description
A probe scans the surface of a moon, returning the elevation profile of crater rims and floors. Ice is believed to be trapped in the shadowed depressions between high crater rims. Calculate the potential volume of ice deposits based on the terrain's capacity to 'trap' material.

## Examples

### 1

#### Input
12
0 1 0 2 1 0 1 3 2 1 2 1

#### Output
6

#### Explanation
Total trapped units = 1 + 1 + 2 + 1 + 1 = 6.

### 2

#### Input
6
4 2 0 3 2 5

#### Output
9

#### Explanation
Total trapped units = 2 + 4 + 1 + 2 = 9.

## Input Format
- The first line contains a single integer n, the number of elements.
- The second line contains n space-separated non-negative integers, representing the profile heights from left to right.

## Output Format
- Return a single integer representing the total accumulated capacity.

## Constraints
- 1 ≤ n ≤ 1e5
- 0 ≤ height ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, stack, dynamic-programming
