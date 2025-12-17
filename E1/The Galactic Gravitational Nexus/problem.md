## Title
The Galactic Gravitational Nexus

## Slug
galactic-gravitational-nexus

## Difficulty
Easy

## Description
In the year 3042, the Interstellar Alliance is constructing a new hyper-lane gate. To ensure the gate does not tear apart due to tidal forces, it must be placed at a specific point in a line of celestial bodies. You are the Chief Astrogator. You have scanned a sector and received a sequence of gravitational readings (positive for matter, negative for exotic matter). You need to find the specific location (index) in this sequence where the gravitational pull from all bodies to the 'West' perfectly cancels out the gravitational pull from all bodies to the 'East'. The gate itself has negligible mass and does not contribute to the calculation.

You are given an array `nums` representing gravitational readings of celestial bodies aligned in a sector. A Stability Nexus is an index where the sum of all gravitational pulls strictly to its left is equal to the sum of all gravitational pulls strictly to its right. If the pivot lies at an edge, the missing side is treated as having a sum of 0. Your task is to return the leftmost such Stability Nexus. If no such point exists, return -1.

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
Both sides are equal, so index 3 is a Stability Nexus.
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
Both sides are equal, so index 0 is a Stability Nexus.
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
