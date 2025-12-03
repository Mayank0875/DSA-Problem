## Title
Cargo Ship Containers

## Slug
cargo-ship-containers

## Difficulty
Hard

## Description
n containers are on a ship. Locks connect some into stacks. The captain wants stacks of 'Load Size' (digits 4 and 7).

You can add locks. Merging k stacks requires k - 1 locks.

Your task is to determine the minimum number of extra locks the captain needs to build to create at least one stack whose size is a Load Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect container 4 with container 3. We can also connect 4 with 1 or 2. This creates a stack of size 4 (a Load Size).

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
There is no way to connect the containers to form a stack with a size equal to a Load Size.

## Input Format
- The first line contains two integers n and m: the number of containers and the number of existing locks.
- The next m lines each contain two integers u and v, representing a lock between container u and container v. Note that u may be equal to v, and there may be multiple locks connecting the same pair of containers.

## Output Format
- Return a single integer: the minimum number of locks to build. If no solution exists, print -1.

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
