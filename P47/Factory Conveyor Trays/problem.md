## Title
Factory Conveyor Trays

## Slug
factory-conveyor-trays

## Difficulty
Easy

## Description
A manufacturing plant uses trays on a conveyor belt to move parts. Each tray has slots for two parts and a weight limit. Given the weights of the parts produced, find the minimum number of trays required to move the batch.

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
