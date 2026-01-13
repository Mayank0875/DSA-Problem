## Title
Missing Library Volume

## Slug
missing-library-volume

## Difficulty
Medium

## Description
A librarian is organizing a series of encyclopedias. The volumes should be numbered sequentially starting from 1. However, the collection is messy, and some volumes are missing or have invalid negative codes.

You are given an unsorted integer array `ids` representing the Volume Numbers currently in the system. Some Volume Numbers may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Volume Number that is **missing** from the list. This will be the next volume number to acquire.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Volume Numbers 1 and 2 are present. The smallest missing positive Volume Number is 3.

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
- Return a single integer representing the smallest missing positive Volume Number.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

