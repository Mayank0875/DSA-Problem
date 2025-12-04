## Title
Forum Threads

## Slug
forum-threads

## Difficulty
Medium

## Description
Discussion threads link to others. A Topic Circle is a group of threads that reference each other.

Two threads a and b belong to the same Topic Circle if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of links.
In other words, two threads are in the same Topic Circle if they are mutually reachable.

Your task is to: Determine how many Topic Circles exist in total.

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
The threads form two distinct groups where round-trip traversal is possible within each group.
Threads {1, 2, 3} form one Topic Circle.
Path: 1 -> 2 -> 3 -> 1.
Threads {4, 5} form another Topic Circle.
Path: 4 -> 5 -> 4.
Total Topic Circles: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 threads and 1 one-way link.
Link: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Topic Circles.

## Input Format
- The first line contains two integers n and m: the number of threads and links.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way link from thread a to thread b.

## Output Format
- Return one integer: the total number of Topic Circles.

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
