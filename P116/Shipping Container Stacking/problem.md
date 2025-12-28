## Title
Shipping Container Stacking

## Slug
shipping-container-stacking

## Difficulty
Medium

## Description
Containers are stacked. Each has a load-bearing range (min weight support, max weight support).

The dock has list of containers, each defined by a min load and an max load, represented as a pair `[min, max]`.

To stack safely, the max load capacity of the lower container must be strictly less than the min load capacity of the upper one (in a specific inverted gravity puzzle). Specifically, to transition from container `[a, b]` to a subsequent container `[c, d]`, the max of the first container must be **strictly less than** the min of the second container (i.e., `b < c`).

You can select containers in any order you like to form a valid stack. Your goal is to determine the maximum number of containers that can be included in a single stack.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest stack is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The containers can be reordered to form the stack `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available containers.
- The next `n` lines each contain two integers, representing the `min` and `max` of an container.

## Output Format
- Return a single integer representing the maximum length of the stack.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ min < max ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
