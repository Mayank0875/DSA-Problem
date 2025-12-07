## Title
Political Alliance

## Slug
political-alliance

## Difficulty
Medium

## Description
Nations sign treaties. An alliance bloc forms when treaties link nations in a circle.

A "alliance bloc" occurs when diplomat moves from a nation, through a sequence of treaties, and returns to the starting nation without traversing the same treaty twice in immediate succession. The "length" of such a alliance bloc is the number of treaties it contains.

Find the size of the smallest alliance bloc.

Given the layout of the geopolitics, determine the length of the shortest alliance bloc.

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
There are several alliance blocs in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest alliance bloc has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no alliance blocs in this network.

## Input Format
- The first line contains two integers n and m: the number of nations and the number of treaties.
- The nations are numbered 1, 2, ..., n.
- The next m lines describe the treaties. Each line contains two integers u and v, indicating a connection between nation u and nation v.
- The graph is undirected. There is at most one treaty between any two nations.

## Output Format
- Return one integer: the length of the shortest alliance bloc. If there are no alliance blocs, print `-1`.

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
