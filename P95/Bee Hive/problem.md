## Title
Bee Hive

## Slug
bee-hive

## Difficulty
Hard

## Description
Pollen is stored in cells. The flavor of a cell is the most frequent flower ID source.

Barry B. Benson has a collection of $n$ pollen grains, where each pollen grain is represented by an integer ID.

To make honey, Barry B. Benson must partition these pollen grains into several non-empty cells. Every pollen grain from the original collection must belong to exactly one cell. From each cell, a "flavor" is extracted. The flavor is defined as the **mode** (most frequent element) of the pollen grains in that cell. If a cell has multiple pollen grains tied for the most frequent appearance, any one of them can be chosen as the flavor.

Barry B. Benson collects all the extracted flavors to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> flavor is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> flavors 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> flavors 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> flavors 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of pollen grains.
- The second line contains $n$ space-separated integers representing the pollen grain IDs.

## Output Format
- Return a single integer representing the number of different multisets of flavors possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
