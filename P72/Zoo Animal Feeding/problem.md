## Title
Zoo Animal Feeding

## Slug
zoo-animal-feeding

## Difficulty
Hard

## Description
A keeper feeds the animals. Starting at the Kitchen (1), they must reach the Staff Room (n). Enclosures are connected by service paths.

The keeper must start at the Kitchen (labeled 1) and finish at the Staff Room (labeled n). However, to place food in every enclosure, the keeper must visit **every single enclosure exactly once** during the journey.

You are given the map of the enclosures and the directed paths connecting them. Your task is to calculate the total number of distinct valid paths the keeper can take to complete the feeding round. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every enclosure exactly once:
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
- The first line contains two integers n and m: the number of enclosures and the number of paths.
- The enclosures are numbered 1, 2, ..., n.
- The next m lines describe the paths. Each line has two integers a and b, indicating a one-way path from enclosure a to enclosure b.

## Output Format
- Return one integer: the number of possible feeding round paths modulo 10^9+7.

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
