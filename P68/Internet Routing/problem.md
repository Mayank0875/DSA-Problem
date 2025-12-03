## Title
Internet Routing

## Slug
internet-routing

## Difficulty
Hard

## Description
n routers manage traffic. Cables connect some into subnets. A protocol works best on subnets of 'Packet Size' (digits 4 and 7).

An admin can plug in cables. Merging k subnets requires k - 1 cables.

Your task is to determine the minimum number of extra cables the admin needs to build to create at least one subnet whose size is a Packet Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect router 4 with router 3. We can also connect 4 with 1 or 2. This creates a subnet of size 4 (a Packet Size).

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
There is no way to connect the routers to form a subnet with a size equal to a Packet Size.

## Input Format
- The first line contains two integers n and m: the number of routers and the number of existing cables.
- The next m lines each contain two integers u and v, representing a cable between router u and router v. Note that u may be equal to v, and there may be multiple cables connecting the same pair of routers.

## Output Format
- Return a single integer: the minimum number of cables to build. If no solution exists, print -1.

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
