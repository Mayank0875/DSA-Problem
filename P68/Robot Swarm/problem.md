## Title
Robot Swarm

## Slug
robot-swarm

## Difficulty
Hard

## Description
n micro-robots are on a floor. Magnetic locks connect them into swarms. The Hive Mind optimizes swarms of 'Prime-Like Size' (digits 4 and 7).

You can command locks to engage. Merging k swarms requires k - 1 commands.

Your task is to determine the minimum number of extra commands the Hive Mind needs to build to create at least one swarm whose size is a Prime-Like Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect robot 4 with robot 3. We can also connect 4 with 1 or 2. This creates a swarm of size 4 (a Prime-Like Size).

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
There is no way to connect the robots to form a swarm with a size equal to a Prime-Like Size.

## Input Format
- The first line contains two integers n and m: the number of robots and the number of existing commands.
- The next m lines each contain two integers u and v, representing a lock between robot u and robot v. Note that u may be equal to v, and there may be multiple commands connecting the same pair of robots.

## Output Format
- Return a single integer: the minimum number of commands to build. If no solution exists, print -1.

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
