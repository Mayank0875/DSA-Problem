## Title
Elevator Floor Button

## Slug
elevator-floor-button

## Difficulty
Medium

## Description
An elevator panel has buttons 1, 2, 3... Some buttons are lit (pressed). The system checks for the lowest floor requested that hasn't been visited yet.

You are given an unsorted integer array `ids` representing the Floor Numbers currently in the system. Some Floor Numbers may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Floor Number that is **missing** from the list. This will be the next floor to stop at.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Floor Numbers 1 and 2 are present. The smallest missing positive Floor Number is 3.

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
- Return a single integer representing the smallest missing positive Floor Number.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

