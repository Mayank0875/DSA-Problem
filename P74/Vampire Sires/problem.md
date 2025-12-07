## Title
Vampire Sires

## Slug
vampire-sires

## Difficulty
Medium

## Description
A vampire clan hierarchy is a tree. For a blood ritual, vampires pair up with their direct sire or fledgling. Each vampire can perform the ritual with only one partner.

The structure is a tree with n vampires and n-1 bloodlines.
A ritual pair is formed between two vampires connected by a bloodline.
However, each vampire can be part of at most one ritual pair.

Your task is to calculate the maximum number of ritual pairs that can be formed.

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
One optimal set of ritual pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 ritual pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form ritual pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of vampires.
- The next n-1 lines each contain two integers u and v, representing a bloodline between vampire u and vampire v.

## Output Format
- Return a single integer representing the maximum number of ritual pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
