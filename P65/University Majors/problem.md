## Title
University Majors

## Slug
university-majors

## Difficulty
Medium

## Description
Courses are prerequisites for others. A Core Block is a set of courses that are prerequisites for each other.

Two courses a and b belong to the same Core Block if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of prerequisites.
In other words, two courses are in the same Core Block if they are mutually reachable.

Your task is to: Determine how many Core Blocks exist in total.

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
The courses form two distinct groups where round-trip traversal is possible within each group.
Courses {1, 2, 3} form one Core Block.
Path: 1 -> 2 -> 3 -> 1.
Courses {4, 5} form another Core Block.
Path: 4 -> 5 -> 4.
Total Core Blocks: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 courses and 1 one-way prerequisite.
Prerequisite: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Core Blocks.

## Input Format
- The first line contains two integers n and m: the number of courses and prerequisites.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way prerequisite from course a to course b.

## Output Format
- Return one integer: the total number of Core Blocks.

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
