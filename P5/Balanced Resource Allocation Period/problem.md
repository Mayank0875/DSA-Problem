## Title

Balanced Resource Allocation Period

## Slug

balanced-resource-allocation-period

## Difficulty

Easy

## Description

A system allocates two types of resources, type '0' and type '1', over N time steps. We have a log of which resource type was allocated at each step. We need to find the longest continuous time period during which the total allocation count for type '0' resources was equal to the total allocation count for type '1' resources. This indicates a balanced allocation phase. Determine the length of the longest such period.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The period [0, 1] shows one allocation of each type, making it the longest balanced period.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

Periods [0, 1] and [1, 0] are the longest balanced allocation periods.

## Input Format

- The first line contains a single integer N, the number of time steps.
- The second line contains N space-separated integers, representing the resource type allocated (0 or 1).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced allocation period.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, resource management, prefix sum, hashmap