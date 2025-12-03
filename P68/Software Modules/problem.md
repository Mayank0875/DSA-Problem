## Title
Software Modules

## Slug
software-modules

## Difficulty
Hard

## Description
n code modules are in a project. Dependencies connect some into libraries. The architect wants libraries of 'Clean Size' (digits 4 and 7).

You can add dependencies. Merging k libraries requires k - 1 new dependencies.

Your task is to determine the minimum number of extra dependencies the architect needs to build to create at least one library whose size is a Clean Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect module 4 with module 3. We can also connect 4 with 1 or 2. This creates a library of size 4 (a Clean Size).

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
There is no way to connect the modules to form a library with a size equal to a Clean Size.

## Input Format
- The first line contains two integers n and m: the number of modules and the number of existing dependencies.
- The next m lines each contain two integers u and v, representing a dependency between module u and module v. Note that u may be equal to v, and there may be multiple dependencies connecting the same pair of modules.

## Output Format
- Return a single integer: the minimum number of dependencies to build. If no solution exists, print -1.

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
