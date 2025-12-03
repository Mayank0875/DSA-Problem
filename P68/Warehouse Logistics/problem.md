## Title
Warehouse Logistics

## Slug
warehouse-logistics

## Difficulty
Hard

## Description
n storage bins are in a depot. Conveyors link some into zones. Efficiency is highest for zones of 'Cargo Size' (digits 4 and 7).

A manager can add conveyors. Merging k zones costs k - 1 conveyors.

Your task is to determine the minimum number of extra conveyors the manager needs to build to create at least one zone whose size is a Cargo Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect bin 4 with bin 3. We can also connect 4 with 1 or 2. This creates a zone of size 4 (a Cargo Size).

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
There is no way to connect the bins to form a zone with a size equal to a Cargo Size.

## Input Format
- The first line contains two integers n and m: the number of bins and the number of existing conveyors.
- The next m lines each contain two integers u and v, representing a conveyor between bin u and bin v. Note that u may be equal to v, and there may be multiple conveyors connecting the same pair of bins.

## Output Format
- Return a single integer: the minimum number of conveyors to build. If no solution exists, print -1.

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
