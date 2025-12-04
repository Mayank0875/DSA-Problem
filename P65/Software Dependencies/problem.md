## Title
Software Dependencies

## Slug
software-dependencies

## Difficulty
Medium

## Description
Software modules depend on others. A Cyclic Dependency Group is a set of modules that depend on each other.

Two modules a and b belong to the same Dependency Group if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of dependencies.
In other words, two modules are in the same Dependency Group if they are mutually reachable.

Your task is to: Determine how many Dependency Groups exist in total.

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
The modules form two distinct groups where round-trip traversal is possible within each group.
Modules {1, 2, 3} form one Dependency Group.
Path: 1 -> 2 -> 3 -> 1.
Modules {4, 5} form another Dependency Group.
Path: 4 -> 5 -> 4.
Total Dependency Groups: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 modules and 1 one-way dependency.
Dependency: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Dependency Groups.

## Input Format
- The first line contains two integers n and m: the number of modules and dependencies.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way dependency from module a to module b.

## Output Format
- Return one integer: the total number of Dependency Groups.

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
