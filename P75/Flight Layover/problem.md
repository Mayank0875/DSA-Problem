## Title
Flight Layover

## Slug
flight-layover

## Difficulty
Medium

## Description
A traveler looks at flight maps. An itinerary that returns to the starting airport is a round-the-world trip.

A "itinerary loop" occurs when a passenger moves from a airport, through a sequence of flights, and returns to the starting airport without traversing the same flight twice in immediate succession. The "length" of such a itinerary loop is the number of flights it contains.

Find the fewest number of flights to make a round trip.

Given the layout of the flight map, determine the length of the shortest itinerary loop.

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
There are several itinerary loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest itinerary loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no itinerary loops in this network.

## Input Format
- The first line contains two integers n and m: the number of airports and the number of flights.
- The airports are numbered 1, 2, ..., n.
- The next m lines describe the flights. Each line contains two integers u and v, indicating a connection between airport u and airport v.
- The graph is undirected. There is at most one flight between any two airports.

## Output Format
- Return one integer: the length of the shortest itinerary loop. If there are no itinerary loops, print `-1`.

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
