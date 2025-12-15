## Title
Bank Vault Tunnel

## Slug
bank-vault-tunnel

## Difficulty
Medium

## Description
Thieves are digging from a Shop (node 1) to the Vault (node n).

The underground consists of $n$ basements connected by $m$ two-way tunnels.
The thieves is attempting to travel from the Shop (node 1) to the Vault (node $n$).

To prevent this, you can collapse specific tunnels. Collapsing a tunnel stops them.

Your task is to calculate the **minimum number of tunnels** that must be collapsed to completely sever all routes between the Shop and the Vault.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can collapse edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of basements and tunnels.
- The next $m$ lines describe the tunnels. Each line contains two integers $a$ and $b$, indicating a tunnel between basement $a$ and basement $b$.

## Output Format
- Return one integer: the minimum number of tunnels that need to be collapsed.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
