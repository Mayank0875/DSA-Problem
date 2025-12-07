## Title
Lost Hiker

## Slug
lost-hiker

## Difficulty
Medium

## Description
A hiker is lost in the woods. They accidentally walk a path that leads them back to a landmark they already passed.

A "circle" occurs when the hiker moves from a clearing, through a sequence of paths, and returns to the starting clearing without traversing the same path twice in immediate succession. The "length" of such a circle is the number of paths it contains.

Walking in tight circles is frustrating. Find the length of the shortest circular hike.

Given the layout of the forest, determine the length of the shortest circle.

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
There are several circles in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest circle has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no circles in this network.

## Input Format
- The first line contains two integers n and m: the number of clearings and the number of paths.
- The clearings are numbered 1, 2, ..., n.
- The next m lines describe the paths. Each line contains two integers u and v, indicating a connection between clearing u and clearing v.
- The graph is undirected. There is at most one path between any two clearings.

## Output Format
- Return one integer: the length of the shortest circle. If there are no circles, print `-1`.

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
