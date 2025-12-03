## Title
Military Platoon

## Slug
military-platoon

## Difficulty
Hard

## Description
An army has n squads. Communication lines link some squads into platoons. Strategic doctrine states a platoon is optimal if its squad count is a 'Tactical Number' (digits 4 and 7).

The general wants to lay new lines to merge platoons. Merging k platoons takes k - 1 new lines.

Your task is to determine the minimum number of extra lines the general needs to build to create at least one platoon whose size is a Tactical Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect squad 4 with squad 3. We can also connect 4 with 1 or 2. This creates a platoon of size 4 (a Tactical Number).

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
There is no way to connect the squads to form a platoon with a size equal to a Tactical Number.

## Input Format
- The first line contains two integers n and m: the number of squads and the number of existing lines.
- The next m lines each contain two integers u and v, representing a line between squad u and squad v. Note that u may be equal to v, and there may be multiple lines connecting the same pair of squads.

## Output Format
- Return a single integer: the minimum number of lines to build. If no solution exists, print -1.

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
