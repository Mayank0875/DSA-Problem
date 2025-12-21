## Title
Mineral Refining

## Slug
mineral-refining

## Difficulty
Hard

## Description
Raw ores are smelted in batches. The resulting ingot type is determined by the most abundant mineral ID in the batch.

The Smith has a collection of $n$ ores, where each ore is represented by an integer ID.

To forge alloys, The Smith must partition these ores into several non-empty batches. Every ore from the original collection must belong to exactly one batch. From each batch, a "ingot type" is extracted. The ingot type is defined as the **mode** (most frequent element) of the ores in that batch. If a batch has multiple ores tied for the most frequent appearance, any one of them can be chosen as the ingot type.

The Smith collects all the extracted ingot types to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> ingot type is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> ingot types 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> ingot types 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> ingot types 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of ores.
- The second line contains $n$ space-separated integers representing the ore IDs.

## Output Format
- Return a single integer representing the number of different multisets of ingot types possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
