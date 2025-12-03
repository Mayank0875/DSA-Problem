## Title
Volcanic Islands

## Slug
volcanic-islands

## Difficulty
Hard

## Description
n volcanic vents are on the ocean floor. Lava tubes connect some into systems. Geologists study systems of 'Magma Number' (digits 4 and 7).

You can map tubes. Merging k systems requires k - 1 mapping expeditions.

Your task is to determine the minimum number of extra expeditions the geologist needs to build to create at least one system whose size is a Magma Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect vent 4 with vent 3. We can also connect 4 with 1 or 2. This creates a system of size 4 (a Magma Number).

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
There is no way to connect the vents to form a system with a size equal to a Magma Number.

## Input Format
- The first line contains two integers n and m: the number of vents and the number of existing expeditions.
- The next m lines each contain two integers u and v, representing a tube between vent u and vent v. Note that u may be equal to v, and there may be multiple expeditions connecting the same pair of vents.

## Output Format
- Return a single integer: the minimum number of expeditions to build. If no solution exists, print -1.

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
