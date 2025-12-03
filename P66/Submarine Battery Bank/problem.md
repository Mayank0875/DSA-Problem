## Title
Submarine Battery Bank

## Slug
submarine-battery-bank

## Difficulty
Medium

## Description
Two banks of batteries need cross-connections to power the sub if a cell dies.

Two parallel banks, Port Bank and Starboard Bank, each contain n cells arranged in a line.
Port Bank has an array `a` representing the charge level of each cell.
Starboard Bank has an array `b` representing the charge level of each cell.

Inside each bank, adjacent cells are already connected by internal bus bars.

You must establish inter-bank jumpers connecting some cells of Port Bank to some cells of Starboard Bank.

The cost to create a jumper between cell i of Port Bank and cell j of Starboard Bank is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single cell is removed (from either Port Bank or Starboard Bank).
If one cell fails and disappears along with all its connections, the remaining cells must still form a single connected network.

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
It's optimal to connect four pairs of cells:
1. cell 1 from Port Bank with cell 2 from Starboard Bank: cost |1-4| = 3.
2. cell 3 from Port Bank with cell 2 from Starboard Bank: cost |1-4| = 3.
3. cell 2 from Port Bank with cell 1 from Starboard Bank: cost |10-20| = 10.
4. cell 2 from Port Bank with cell 3 from Starboard Bank: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first cell of Port Bank with the first of Starboard Bank, and the last cell of Port Bank with the last of Starboard Bank, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of cells in each bank.
- The second line contains n integers representing the charge levels of Port Bank.
- The third line contains n integers representing the charge levels of Starboard Bank.

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
