## Title
Castle Wall

## Slug
castle-wall

## Difficulty
Medium

## Description
An architect designs a castle. The walls must form a closed perimeter.

A "perimeter" occurs when a guard moves from a tower, through a sequence of sections, and returns to the starting tower without traversing the same wall section twice in immediate succession. The "length" of such a perimeter is the number of sections it contains.

A small inner keep provides a last defense. Find the length of the smallest walled enclosure.

Given the layout of the fortress, determine the length of the shortest perimeter.

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
There are several perimeters in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest perimeter has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no perimeters in this network.

## Input Format
- The first line contains two integers n and m: the number of towers and the number of sections.
- The towers are numbered 1, 2, ..., n.
- The next m lines describe the sections. Each line contains two integers u and v, indicating a connection between tower u and tower v.
- The graph is undirected. There is at most one wall section between any two towers.

## Output Format
- Return one integer: the length of the shortest perimeter. If there are no perimeters, print `-1`.

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
