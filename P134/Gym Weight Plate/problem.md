## Title
Gym Weight Plate

## Slug
gym-weight-plate

## Difficulty
Medium

## Description
Weight plates are labeled 1kg, 2kg, 3kg... (simplified). A lifter has a pile of plates. Which is the lightest plate they are missing?

You are given an unsorted integer array `ids` representing the Weights currently in the system. Some Weights may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Weight that is **missing** from the list. This will be the missing weight.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Weights 1 and 2 are present. The smallest missing positive Weight is 3.

### 2

#### Input
4
3 4 -1 1

#### Output
2

#### Explanation
1 is present, but 2 is missing.

## Input Format
- The first line contains an integer $n$, the size of the array.
- The second line contains $n$ space-separated integers `ids`.

## Output Format
- Return a single integer representing the smallest missing positive Weight.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

