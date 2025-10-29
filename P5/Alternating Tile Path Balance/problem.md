## Title

Alternating Tile Path Balance

## Slug

alternating-tile-path-balance

## Difficulty

Easy

## Description

You are walking along a path paved with black ('0') and white ('1') tiles. You want to find the longest continuous section of the path you walked on that contains exactly the same number of black tiles as white tiles. This represents the longest section with perfect color balance. Given the sequence of tile colors along your path, find the length of this longest balanced section.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The section [0, 1] (Black, White) is the longest with equal numbers of black and white tiles.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Black, White) and [1, 0] (White, Black) are the longest balanced sections.

## Input Format

- The first line contains a single integer N, the total number of tiles on the path.
- The second line contains N space-separated integers, representing the tile colors (0 for black, 1 for white).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced section.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hashmap