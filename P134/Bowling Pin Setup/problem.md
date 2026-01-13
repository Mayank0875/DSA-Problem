## Title
Bowling Pin Setup

## Slug
bowling-pin-setup

## Difficulty
Medium

## Description
Bowling pins are numbered 1 to 10 (or higher in this variant). A machine checks which pins are standing. Find the lowest numbered pin that has been knocked down.

You are given an unsorted integer array `ids` representing the Pin Numbers currently in the system. Some Pin Numbers may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Pin Number that is **missing** from the list. This will be the number of the fallen pin.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Pin Numbers 1 and 2 are present. The smallest missing positive Pin Number is 3.

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
- Return a single integer representing the smallest missing positive Pin Number.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

