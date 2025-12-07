## Title
Logistics Return Route

## Slug
logistics-return-route

## Difficulty
Medium

## Description
Delivery trucks need efficient routes. A route that ends where it started is a round-trip.

A "round-trip" occurs when a truck moves from a warehouse, through a sequence of highways, and returns to the starting warehouse without traversing the same highway twice in immediate succession. The "length" of such a round-trip is the number of highways it contains.

Short round-trips are efficient for local distribution. Find the shortest round-trip distance.

Given the layout of the logistics map, determine the length of the shortest round-trip.

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
There are several round-trips in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest round-trip has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no round-trips in this network.

## Input Format
- The first line contains two integers n and m: the number of warehouses and the number of highways.
- The warehouses are numbered 1, 2, ..., n.
- The next m lines describe the highways. Each line contains two integers u and v, indicating a connection between warehouse u and warehouse v.
- The graph is undirected. There is at most one highway between any two warehouses.

## Output Format
- Return one integer: the length of the shortest round-trip. If there are no round-trips, print `-1`.

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
