## Title
Space Fleet

## Slug
space-fleet

## Difficulty
Hard

## Description
Ships are organized into squadrons. The flagship class of a squadron is the most common ship class ID within it.

Admiral Ackbar has a collection of $n$ ships, where each ship is represented by an integer ID.

To plan the defense, Admiral Ackbar must partition these ships into several non-empty squadrons. Every ship from the original collection must belong to exactly one squadron. From each squadron, a "flagship class" is extracted. The flagship class is defined as the **mode** (most frequent element) of the ships in that squadron. If a squadron has multiple ships tied for the most frequent appearance, any one of them can be chosen as the flagship class.

Admiral Ackbar collects all the extracted flagship classs to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> flagship class is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> flagship classs 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> flagship classs 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> flagship classs 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of ships.
- The second line contains $n$ space-separated integers representing the ship IDs.

## Output Format
- Return a single integer representing the number of different multisets of flagship classs possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
