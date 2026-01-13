## Title
Card Collection Gap

## Slug
card-collection-gap

## Difficulty
Medium

## Description
A collector has a set of numbered trading cards. They want to know the first card number (starting from 1) they are missing to complete the early part of the set.

You are given an unsorted integer array `ids` representing the Card Numbers currently in the system. Some Card Numbers may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Card Number that is **missing** from the list. This will be the number of the first missing card.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Card Numbers 1 and 2 are present. The smallest missing positive Card Number is 3.

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
- Return a single integer representing the smallest missing positive Card Number.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

