## Title
Galaxy Clusters

## Slug
galaxy-clusters

## Difficulty
Hard

## Description
Stars are grouped into sectors. The classification of a sector is the most common star type ID within it.

The Astronomer has a collection of $n$ stars, where each star is represented by an integer ID.

To map the universe, The Astronomer must partition these stars into several non-empty sectors. Every star from the original collection must belong to exactly one sector. From each sector, a "classification" is extracted. The classification is defined as the **mode** (most frequent element) of the stars in that sector. If a sector has multiple stars tied for the most frequent appearance, any one of them can be chosen as the classification.

The Astronomer collects all the extracted classifications to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> classification is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> classifications 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> classifications 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> classifications 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of stars.
- The second line contains $n$ space-separated integers representing the star IDs.

## Output Format
- Return a single integer representing the number of different multisets of classifications possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
