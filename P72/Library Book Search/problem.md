## Title
Library Book Search

## Slug
library-book-search

## Difficulty
Hard

## Description
A student searches for a book. Starting at the Lobby (1), they must reach the Reading Room (n). Sections are connected by aisles.

The student must start at the Lobby (labeled 1) and finish at the Reading Room (labeled n). However, to check the catalog in every section, the student must visit **every single section exactly once** during the journey.

You are given the map of the sections and the directed aisles connecting them. Your task is to calculate the total number of distinct valid paths the student can take to complete the search. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every section exactly once:
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
- The first line contains two integers n and m: the number of sections and the number of aisles.
- The sections are numbered 1, 2, ..., n.
- The next m lines describe the aisles. Each line has two integers a and b, indicating a one-way aisle from section a to section b.

## Output Format
- Return one integer: the number of possible search paths modulo 10^9+7.

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
