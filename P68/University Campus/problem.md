## Title
University Campus

## Slug
university-campus

## Difficulty
Hard

## Description
n buildings are on campus. Paths connect some into quads. The dean wants quads of 'Student Capacity' (digits 4 and 7).

You can pave paths. Merging k quads costs k - 1 paths.

Your task is to determine the minimum number of extra paths the dean needs to build to create at least one quad whose size is a Student Capacity. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect building 4 with building 3. We can also connect 4 with 1 or 2. This creates a quad of size 4 (a Student Capacity).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the buildings to form a quad with a size equal to a Student Capacity.

## Input Format
- The first line contains two integers n and m: the number of buildings and the number of existing paths.
- The next m lines each contain two integers u and v, representing a path between building u and building v. Note that u may be equal to v, and there may be multiple paths connecting the same pair of buildings.

## Output Format
- Return a single integer: the minimum number of paths to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
