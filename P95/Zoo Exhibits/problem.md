## Title
Zoo Exhibits

## Slug
zoo-exhibits

## Difficulty
Hard

## Description
Animals are placed into enclosures. The theme of an enclosure is the most common animal species ID within it.

Zookeeper Jane has a collection of $n$ animals, where each animal is represented by an integer ID.

To design the park, Zookeeper Jane must partition these animals into several non-empty enclosures. Every animal from the original collection must belong to exactly one enclosure. From each enclosure, a "theme" is extracted. The theme is defined as the **mode** (most frequent element) of the animals in that enclosure. If a enclosure has multiple animals tied for the most frequent appearance, any one of them can be chosen as the theme.

Zookeeper Jane collects all the extracted themes to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> theme is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> themes 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> themes 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> themes 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of animals.
- The second line contains $n$ space-separated integers representing the animal IDs.

## Output Format
- Return a single integer representing the number of different multisets of themes possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
