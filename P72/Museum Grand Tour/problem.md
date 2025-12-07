## Title
Museum Grand Tour

## Slug
museum-grand-tour

## Difficulty
Hard

## Description
A museum has opened a special exhibition. Visitors enter at Hall 1 and leave at Hall n. The halls are connected by one-way corridors.

The visitor must start at the Entrance Hall (labeled 1) and finish at the Exit Hall (labeled n). However, to see every exhibit piece without backtracking, the visitor must visit **every single hall exactly once** during the journey.

You are given the map of the halls and the directed corridors connecting them. Your task is to calculate the total number of distinct valid paths the visitor can take to complete the tour. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every hall exactly once:
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
- The first line contains two integers n and m: the number of halls and the number of corridors.
- The halls are numbered 1, 2, ..., n.
- The next m lines describe the corridors. Each line has two integers a and b, indicating a one-way corridor from hall a to hall b.

## Output Format
- Return one integer: the number of possible tour paths modulo 10^9+7.

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
