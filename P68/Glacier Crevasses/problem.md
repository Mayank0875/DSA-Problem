## Title
Glacier Crevasses

## Slug
glacier-crevasses

## Difficulty
Hard

## Description
n ice patches are on a glacier. Frozen bridges connect some into fields. An explorer seeks fields of 'Ice Number' size (digits 4 and 7).

You can place ladders. Merging k fields requires k - 1 ladders.

Your task is to determine the minimum number of extra ladders the explorer needs to build to create at least one field whose size is a Ice Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect ice patch 4 with ice patch 3. We can also connect 4 with 1 or 2. This creates a field of size 4 (a Ice Number).

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
There is no way to connect the patches to form a field with a size equal to a Ice Number.

## Input Format
- The first line contains two integers n and m: the number of patches and the number of existing ladders.
- The next m lines each contain two integers u and v, representing a bridge between ice patch u and ice patch v. Note that u may be equal to v, and there may be multiple ladders connecting the same pair of patches.

## Output Format
- Return a single integer: the minimum number of ladders to build. If no solution exists, print -1.

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
