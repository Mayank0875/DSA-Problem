## Title
Constellation Mapping

## Slug
constellation-mapping

## Difficulty
Hard

## Description
An astronomer traces a mythical creature in the stars. Starting at Star 1, the line ends at Star n. The stars are linked by imaginary celestial lines.

The astronomer must start at the Head Star (labeled 1) and finish at the Tail Star (labeled n). However, to include every star in the constellation, the astronomer must visit **every single star exactly once** during the journey.

You are given the map of the stars and the directed lines connecting them. Your task is to calculate the total number of distinct valid paths the astronomer can take to complete the mapping. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every star exactly once:
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
- The first line contains two integers n and m: the number of stars and the number of lines.
- The stars are numbered 1, 2, ..., n.
- The next m lines describe the lines. Each line has two integers a and b, indicating a one-way line from star a to star b.

## Output Format
- Return one integer: the number of possible mapping paths modulo 10^9+7.

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
