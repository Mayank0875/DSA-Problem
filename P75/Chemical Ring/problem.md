## Title
Chemical Ring

## Slug
chemical-ring

## Difficulty
Medium

## Description
Chemists are analyzing a molecular structure. Atoms are bonded together, and sometimes they form rings.

A "ring" occurs when a charge moves from a atom, through a sequence of bonds, and returns to the starting atom without traversing the same bond twice in immediate succession. The "length" of such a ring is the number of bonds it contains.

Small rings are often unstable. Your task is to find the number of atoms in the smallest ring structure.

Given the layout of the molecule, determine the length of the shortest ring.

## Examples

### 1

#### Input
5 6
1 2
1 3
2 4
2 5
3 4
4 5

#### Output
3

#### Explanation
There are several rings in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest ring has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no rings in this network.

## Input Format
- The first line contains two integers n and m: the number of atoms and the number of bonds.
- The atoms are numbered 1, 2, ..., n.
- The next m lines describe the bonds. Each line contains two integers u and v, indicating a connection between atom u and atom v.
- The graph is undirected. There is at most one bond between any two atoms.

## Output Format
- Return one integer: the length of the shortest ring. If there are no rings, print `-1`.

## Constraints
- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
