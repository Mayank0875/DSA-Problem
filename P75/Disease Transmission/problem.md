## Title
Disease Transmission

## Slug
disease-transmission

## Difficulty
Medium

## Description
Epidemiologists trace contacts. A transmission ring occurs if the virus infects a chain of people ending back at the start.

A "infection ring" occurs when the virus moves from a person, through a sequence of contacts, and returns to the starting person without traversing the same contact twice in immediate succession. The "length" of such a infection ring is the number of contacts it contains.

Small rings create localized outbreaks. Find the size of the smallest infection ring.

Given the layout of the population, determine the length of the shortest infection ring.

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
There are several infection rings in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest infection ring has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no infection rings in this network.

## Input Format
- The first line contains two integers n and m: the number of people and the number of contacts.
- The people are numbered 1, 2, ..., n.
- The next m lines describe the contacts. Each line contains two integers u and v, indicating a connection between person u and person v.
- The graph is undirected. There is at most one contact between any two people.

## Output Format
- Return one integer: the length of the shortest infection ring. If there are no infection rings, print `-1`.

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
