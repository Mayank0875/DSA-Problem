## Title
Robot Assembly

## Slug
robot-assembly

## Difficulty
Hard

## Description
Parts are kitted for assembly. The model of a kit is defined by the most frequent part ID it contains.

The Engineer has a collection of $n$ parts, where each part is represented by an integer ID.

To build robots, The Engineer must partition these parts into several non-empty kits. Every part from the original collection must belong to exactly one kit. From each kit, a "model ID" is extracted. The model ID is defined as the **mode** (most frequent element) of the parts in that kit. If a kit has multiple parts tied for the most frequent appearance, any one of them can be chosen as the model ID.

The Engineer collects all the extracted model IDs to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> model ID is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> model IDs 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> model IDs 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> model IDs 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of parts.
- The second line contains $n$ space-separated integers representing the part IDs.

## Output Format
- Return a single integer representing the number of different multisets of model IDs possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
