## Title
Family Tree Loop

## Slug
family-tree-loop

## Difficulty
Medium

## Description
Genealogists map relations. Inbreeding loops occur when relatives marry relatives.

A "consanguinity loop" occurs when lineage moves from a person, through a sequence of relations, and returns to the starting person without traversing the same relation twice in immediate succession. The "length" of such a consanguinity loop is the number of relations it contains.

Find the size of the tightest family loop.

Given the layout of the family tree, determine the length of the shortest consanguinity loop.

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
There are several consanguinity loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest consanguinity loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no consanguinity loops in this network.

## Input Format
- The first line contains two integers n and m: the number of people and the number of relations.
- The people are numbered 1, 2, ..., n.
- The next m lines describe the relations. Each line contains two integers u and v, indicating a connection between person u and person v.
- The graph is undirected. There is at most one relation between any two people.

## Output Format
- Return one integer: the length of the shortest consanguinity loop. If there are no consanguinity loops, print `-1`.

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
