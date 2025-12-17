## Title
The Structural Beam Analysis

## Slug
structural-beam-analysis

## Difficulty
Easy

## Description
Civil engineers are analyzing a long steel beam used in a skyscraper. The beam has several joints, and at each joint, various forces are applied (wind load, weight load, tension). These forces are mapped as an array of integers. To install the primary safety sensor, the engineers need to identify the 'Equilibrium Joint'. This is the joint where the sum of all forces acting on the left side of the beam is equal to the sum of all forces acting on the right side. Installing the sensor here ensures the most accurate reading of the building's structural integrity.

You are given an array `nums` representing stress loads on a steel beam. A Equilibrium Joint is an index where the sum of all force vectors strictly to its left is equal to the sum of all force vectors strictly to its right. If the pivot lies at an edge, the missing side is treated as having a sum of 0. Your task is to return the leftmost such Equilibrium Joint. If no such point exists, return -1.

## Examples

### 1

#### Input

nums = [1, 7, 3, 6, 5, 6]

#### Output

3

#### Explanation

For index 3 (value = 6):
Left side sum = 1 + 7 + 3 = 11
Right side sum = 5 + 6 = 11
Both sides are equal, so index 3 is a Equilibrium Joint.
It is also the leftmost such index.


### 2

#### Input

nums = [1, 2, 3]

#### Output

-1

#### Explanation

Index 0: left sum = 0, right sum = 2 + 3 = 5 (not equal)
Index 1: left sum = 1, right sum = 3 (not equal)
Index 2: left sum = 1 + 2 = 3, right sum = 0 (not equal)
No index has equal left and right sum, so answer is -1.


### 3

#### Input

nums = [2, 1, -1]

#### Output

0

#### Explanation

At index 0:
Left sum = 0
Right sum = 1 + (-1) = 0
Both sides are equal, so index 0 is a Equilibrium Joint.
Since it is the first index, it is the leftmost pivot.


## Input Format

- A single line containing an integer array `nums`.

## Output Format

- Return the index representing the leftmost pivot, or -1 if no such pivot exists.

## Constraints

- 1 ≤ nums.length ≤ 10⁴
- -1000 ≤ nums[i] ≤ 1000

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

array, prefix-sum
