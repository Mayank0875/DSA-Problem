## Title
Corporate Departments

## Slug
corporate-departments

## Difficulty
Medium

## Description
In a company, N employees forward emails. An Information Silo is a group of employees who can all forward information to each other indefinitely.

Two employees a and b belong to the same Silo if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of forwards.
In other words, two employees are in the same Silo if they are mutually reachable.

Your task is to: Determine how many Silos exist in total.

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
The employees form two distinct groups where round-trip traversal is possible within each group.
Employees {1, 2, 3} form one Silo.
Path: 1 -> 2 -> 3 -> 1.
Employees {4, 5} form another Silo.
Path: 4 -> 5 -> 4.
Total Silos: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 employees and 1 one-way forward.
Forward: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Silos.

## Input Format
- The first line contains two integers n and m: the number of employees and forwards.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way forward from employee a to employee b.

## Output Format
- Return one integer: the total number of Silos.

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
