## Title
Mining Shafts

## Slug
mining-shafts

## Difficulty
Hard

## Description
n ore deposits are found. Tunnels connect some into mines. The foreman targets mines of 'Yield Size' (digits 4 and 7).

Miners can dig tunnels. Merging k mines requires k - 1 tunnels.

Your task is to determine the minimum number of extra tunnels the foreman needs to build to create at least one mine whose size is a Yield Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect deposit 4 with deposit 3. We can also connect 4 with 1 or 2. This creates a mine of size 4 (a Yield Size).

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
There is no way to connect the deposits to form a mine with a size equal to a Yield Size.

## Input Format
- The first line contains two integers n and m: the number of deposits and the number of existing tunnels.
- The next m lines each contain two integers u and v, representing a tunnel between deposit u and deposit v. Note that u may be equal to v, and there may be multiple tunnels connecting the same pair of deposits.

## Output Format
- Return a single integer: the minimum number of tunnels to build. If no solution exists, print -1.

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
