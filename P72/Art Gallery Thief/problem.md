## Title
Art Gallery Thief

## Slug
art-gallery-thief

## Difficulty
Hard

## Description
A thief sneaks through a gallery. Starting at the Window (1), they must reach the Roof (n). Exhibit rooms are connected by doors.

The thief must start at the Window (labeled 1) and finish at the Roof (labeled n). However, to steal one item from every room, the thief must visit **every single room exactly once** during the journey.

You are given the map of the rooms and the directed doors connecting them. Your task is to calculate the total number of distinct valid paths the thief can take to complete the heist. As the number of paths can be very large, print the answer modulo 1000000007.

## Examples

### 1

#### Input
4 6
1 2
1 3
2 3
3 2
2 4
3 4

#### Output
2

#### Explanation
There are two possible paths that visit every room exactly once:
1 -> 2 -> 3 -> 4
1 -> 3 -> 2 -> 4

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
The only valid path is 1 -> 2.

## Input Format
- The first line contains two integers n and m: the number of rooms and the number of doors.
- The rooms are numbered 1, 2, ..., n.
- The next m lines describe the doors. Each line has two integers a and b, indicating a one-way door from room a to room b.

## Output Format
- Return one integer: the number of possible heist paths modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 20
- 1 ≤ m ≤ n * n
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
