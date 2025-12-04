## Title
Sewer Junctions

## Slug
sewer-junctions

## Difficulty
Medium

## Description
Junctions are connected by pipes. A Drainage Basin is a set of junctions where water can flow cyclically.

Two junctions a and b belong to the same Basin if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of pipes.
In other words, two junctions are in the same Basin if they are mutually reachable.

Your task is to: Determine how many Basins exist in total.

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
The junctions form two distinct groups where round-trip traversal is possible within each group.
Junctions {1, 2, 3} form one Basin.
Path: 1 -> 2 -> 3 -> 1.
Junctions {4, 5} form another Basin.
Path: 4 -> 5 -> 4.
Total Basins: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 junctions and 1 one-way pipe.
Pipe: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Basins.

## Input Format
- The first line contains two integers n and m: the number of junctions and pipes.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way pipe from junction a to junction b.

## Output Format
- Return one integer: the total number of Basins.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
