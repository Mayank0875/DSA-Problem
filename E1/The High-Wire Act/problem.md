## Title
The High-Wire Act

## Slug
high-wire-act

## Difficulty
Easy

## Description
The Great Zampano is attempting a world-record tightrope walk. The rope is fitted with various decorative weights and counter-weights along its length. Before he begins his walk, his engineering team provides him with an array representing the mass of these attachments at specific intervals. Zampano needs to know the exact starting position (index) where he can stand such that the tension pulling him backward is exactly equal to the tension pulling him forward. If he starts at an unbalanced point, the rope might snap or he might lose his balance immediately.

You are given an array `nums` representing ballast weights attached to a tightrope. A Center of Stability is an index where the sum of all weights strictly to its left is equal to the sum of all weights strictly to its right. If the pivot lies at an edge, the missing side is treated as having a sum of 0. Your task is to return the leftmost such Center of Stability. If no such point exists, return -1.

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
Both sides are equal, so index 3 is a Center of Stability.
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
Both sides are equal, so index 0 is a Center of Stability.
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
