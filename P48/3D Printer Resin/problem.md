## Title
3D Printer Resin

## Slug
3d-printer-resin

## Difficulty
Medium

## Description
A 3D printed object has a complex surface profile with ridges of different heights. When dipped in a cleaning resin, the liquid stays trapped in the surface depressions. Calculate the total volume of resin retained by the object's surface profile given the ridge heights.

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
