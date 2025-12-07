## Title
Social Clique

## Slug
social-clique

## Difficulty
Medium

## Description
Sociologists are studying a group of friends. A clique is a chain of friendships that loops back to the start.

A "circle" occurs when a rumor moves from a person, through a sequence of friendships, and returns to the starting person without traversing the same friendship twice in immediate succession. The "length" of such a circle is the number of friendships it contains.

Tight circles spread rumors fastest. Your task is to find the size of the smallest circle of friends.

Given the layout of the social graph, determine the length of the shortest circle.

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
- The first line contains two integers n and m: the number of people and the number of friendships.
- The people are numbered 1, 2, ..., n.
- The next m lines describe the friendships. Each line contains two integers u and v, indicating a connection between person u and person v.
- The graph is undirected. There is at most one friendship between any two people.

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
