## Title
Knight's Castle Quest

## Slug
knights-castle-quest

## Difficulty
Hard

## Description
A knight enters a castle at the Gatehouse (1) and must reach the Throne Room (n). The castle rooms are connected by one-way passages.

The knight must start at the Gatehouse (labeled 1) and finish at the Throne Room (labeled n). However, to clear every room of enemies, the knight must visit **every single room exactly once** during the journey.

You are given the map of the rooms and the directed passages connecting them. Your task is to calculate the total number of distinct valid paths the knight can take to complete the quest. As the number of paths can be very large, print the answer modulo 1000000007.

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
- The first line contains two integers n and m: the number of rooms and the number of passages.
- The rooms are numbered 1, 2, ..., n.
- The next m lines describe the passages. Each line has two integers a and b, indicating a one-way passage from room a to room b.

## Output Format
- Return one integer: the number of possible quest paths modulo 10^9+7.

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
