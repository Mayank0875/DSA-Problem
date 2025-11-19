## Title
Rickshaw Passenger Trips

## Slug
rickshaw-passenger-trips

## Difficulty
Easy

## Description
A rickshaw driver ferries tourists around the city. The rickshaw seats two people max and has a weight limit for the puller's ease. Given the weights of a tour group, calculate the minimum number of trips the driver must make to transport everyone.

## Examples

### 1

#### Input
4 10
7 2 3 9

#### Output
3

#### Explanation
We can group the items as follows:
1. (2, 7) -> sum is 9 <= 10.
2. (3) -> sum is 3 <= 10.
3. (9) -> sum is 9 <= 10.
Total groups = 3.

### 2

#### Input
5 5
2 2 2 3 4

#### Output
3

#### Explanation
We can group the items as follows:
1. (2, 3) -> sum is 5 <= 5.
2. (2, 2) -> sum is 4 <= 5.
3. (4) -> sum is 4 <= 5.
Total groups = 3.

## Input Format
- The first line contains two integers n and x: the number of items and the maximum limit per group.
- The second line contains n integers representing the values/weights of the items.

## Output Format
- Return a single integer: the minimum number of groups required.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ values[i] ≤ x

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, sorting, two pointers
