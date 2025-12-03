## Title
Dungeon Room Sets

## Slug
dungeon-room-sets

## Difficulty
Medium

## Description
A dungeon has N rooms connected by one-way magic portals. A Room Set is a collection of rooms where you can navigate from any room to any other within the set.

Two rooms a and b belong to the same Room Set if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of portals.
In other words, two rooms are in the same Room Set if they are mutually reachable.

Your task is to: Determine how many Room Sets exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The rooms form two distinct groups where round-trip traversal is possible within each group.
Rooms {1, 2, 3} form one Room Set.
Path: 1 -> 2 -> 3 -> 1.
Rooms {4, 5} form another Room Set.
Path: 4 -> 5 -> 4.
Total Room Sets: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 rooms and 1 one-way portal.
Portal: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Room Sets.

## Input Format
- The first line contains two integers n and m: the number of rooms and portals.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way portal from room a to room b.

## Output Format
- Return one integer: the total number of Room Sets.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, strongly-connected-components
