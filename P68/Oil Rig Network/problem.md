## Title
Oil Rig Network

## Slug
oil-rig-network

## Difficulty
Hard

## Description
n rigs are at sea. Pipelines connect some into fields. The company wants fields of 'Barrel Count' (digits 4 and 7).

You can lay pipes. Merging k fields requires k - 1 pipes.

Your task is to determine the minimum number of extra pipes the company needs to build to create at least one field whose size is a Barrel Count. If this goal cannot be achieved, return -1.

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
The optimal way is to connect rig 4 with rig 3. We can also connect 4 with 1 or 2. This creates a field of size 4 (a Barrel Count).

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
There is no way to connect the rigs to form a field with a size equal to a Barrel Count.

## Input Format
- The first line contains two integers n and m: the number of rigs and the number of existing pipes.
- The next m lines each contain two integers u and v, representing a pipe between rig u and rig v. Note that u may be equal to v, and there may be multiple pipes connecting the same pair of rigs.

## Output Format
- Return a single integer: the minimum number of pipes to build. If no solution exists, print -1.

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
