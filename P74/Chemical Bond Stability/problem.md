## Title
Chemical Bond Stability

## Slug
chemical-bond-stability

## Difficulty
Medium

## Description
A complex molecule is represented as a tree of atoms. Chemists want to stabilize the structure by forming double bonds between adjacent atoms. Each atom can participate in only one double bond.

The structure is a tree with n atoms and n-1 bonds.
A double bond is formed between two atoms connected by a bond.
However, each atom can be part of at most one double bond.

Your task is to calculate the maximum number of double bonds that can be formed.

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
One optimal set of double bonds is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 double bonds.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form double bonds (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of atoms.
- The next n-1 lines each contain two integers u and v, representing a bond between atom u and atom v.

## Output Format
- Return a single integer representing the maximum number of double bonds.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
