## Title
The Druid's Mana Convergence

## Slug
druids-mana-convergence

## Difficulty
Easy

## Description
Elara, the High Druid, is preparing for the Solstice Ritual. She has arranged a series of ancient runestones in a straight line across the meadow. Each runestone emits a specific frequency of magical energy (mana). Some stones emit positive healing energy, while others, corrupted by the void, emit negative entropic energy. To open the portal to the Feywild safely, Elara must stand on a specific runestone. This stone must act as a dampener where the cumulative mana flow from the west perfectly balances the cumulative mana flow from the east. If she stands on the wrong stone, the ritual will backfire.

You are given an array `nums` representing runestones lined up in a ritual site. A Convergence Node is an index where the sum of all mana levels strictly to its left is equal to the sum of all mana levels strictly to its right. If the pivot lies at an edge, the missing side is treated as having a sum of 0. Your task is to return the leftmost such Convergence Node. If no such point exists, return -1.

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
Both sides are equal, so index 3 is a Convergence Node.
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
Both sides are equal, so index 0 is a Convergence Node.
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
