## Title
Crystal Resonance

## Slug
crystal-resonance

## Difficulty
Medium

## Description
Magic crystals grow in a tree formation. Resonating pairs can be formed between connected crystals to amplify power. Each crystal can resonate with only one other.

The structure is a tree with n crystals and n-1 growths.
A resonant pair is formed between two crystals connected by a growth.
However, each crystal can be part of at most one resonant pair.

Your task is to calculate the maximum number of resonant pairs that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of resonant pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 resonant pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form resonant pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of crystals.
- The next n-1 lines each contain two integers u and v, representing a growth between crystal u and crystal v.

## Output Format
- Return a single integer representing the maximum number of resonant pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
