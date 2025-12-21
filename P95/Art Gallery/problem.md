## Title
Art Gallery

## Slug
art-gallery

## Difficulty
Hard

## Description
Paintings are hung in rooms. The style of a room is the most frequent art movement ID.

The Curator has a collection of $n$ paintings, where each painting is represented by an integer ID.

To arrange the exhibition, The Curator must partition these paintings into several non-empty rooms. Every painting from the original collection must belong to exactly one room. From each room, a "style" is extracted. The style is defined as the **mode** (most frequent element) of the paintings in that room. If a room has multiple paintings tied for the most frequent appearance, any one of them can be chosen as the style.

The Curator collects all the extracted styles to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> style is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> styles 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> styles 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> styles 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of paintings.
- The second line contains $n$ space-separated integers representing the painting IDs.

## Output Format
- Return a single integer representing the number of different multisets of styles possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
