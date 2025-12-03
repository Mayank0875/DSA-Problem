## Title
River Bridge Network

## Slug
river-bridge-network

## Difficulty
Medium

## Description
Engineers are reinforcing connections between two river banks.

Two parallel banks, North Bank and South Bank, each contain n piers arranged in a line.
North Bank has an array `a` representing the elevation of each pier.
South Bank has an array `b` representing the elevation of each pier.

Inside each bank, adjacent piers are already connected by internal pathways.

You must establish inter-bank bridges connecting some piers of North Bank to some piers of South Bank.

The cost to create a bridge between pier i of North Bank and pier j of South Bank is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single pier is removed (from either North Bank or South Bank).
If one pier fails and disappears along with all its connections, the remaining piers must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of piers:
1. pier 1 from North Bank with pier 2 from South Bank: cost |1-4| = 3.
2. pier 3 from North Bank with pier 2 from South Bank: cost |1-4| = 3.
3. pier 2 from North Bank with pier 1 from South Bank: cost |10-20| = 10.
4. pier 2 from North Bank with pier 3 from South Bank: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first pier of North Bank with the first of South Bank, and the last pier of North Bank with the last of South Bank, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of piers in each bank.
- The second line contains n integers representing the elevations of North Bank.
- The third line contains n integers representing the elevations of South Bank.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
