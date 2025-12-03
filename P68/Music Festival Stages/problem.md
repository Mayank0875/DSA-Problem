## Title
Music Festival Stages

## Slug
music-festival-stages

## Difficulty
Hard

## Description
n stages are set up. Walkways connect some into areas. The organizer wants areas with a 'Vibe Count' of stages (digits 4 and 7).

You can build walkways. Merging k areas costs k - 1 walkways.

Your task is to determine the minimum number of extra walkways the organizer needs to build to create at least one area whose size is a Vibe Count. If this goal cannot be achieved, return -1.

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
The optimal way is to connect stage 4 with stage 3. We can also connect 4 with 1 or 2. This creates a area of size 4 (a Vibe Count).

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
There is no way to connect the stages to form a area with a size equal to a Vibe Count.

## Input Format
- The first line contains two integers n and m: the number of stages and the number of existing walkways.
- The next m lines each contain two integers u and v, representing a walkway between stage u and stage v. Note that u may be equal to v, and there may be multiple walkways connecting the same pair of stages.

## Output Format
- Return a single integer: the minimum number of walkways to build. If no solution exists, print -1.

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
