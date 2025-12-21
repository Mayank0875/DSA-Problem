## Title
Colors of the Wind

## Slug
colors-of-the-wind

## Difficulty
Hard

## Description
Leaves are swept into piles. The color of a pile is determined by the most common leaf color ID found in it.

Pocahontas has a collection of $n$ leaves, where each leaf is represented by an integer ID.

To paint with nature, Pocahontas must partition these leaves into several non-empty piles. Every leaf from the original collection must belong to exactly one pile. From each pile, a "pile color" is extracted. The pile color is defined as the **mode** (most frequent element) of the leaves in that pile. If a pile has multiple leaves tied for the most frequent appearance, any one of them can be chosen as the pile color.

Pocahontas collects all the extracted pile colors to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> pile color is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> pile colors 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> pile colors 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> pile colors 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of leaves.
- The second line contains $n$ space-separated integers representing the leaf IDs.

## Output Format
- Return a single integer representing the number of different multisets of pile colors possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
