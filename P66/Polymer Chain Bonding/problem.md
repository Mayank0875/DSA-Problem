## Title
Polymer Chain Bonding

## Slug
polymer-chain-bonding

## Difficulty
Medium

## Description
Chemical engineers connect two polymer chains to create a durable material resistant to breaking.

Two parallel chains, Polymer A and Polymer B, each contain n monomers arranged in a line.
Polymer A has an array `a` representing the atomic weight of each monomer.
Polymer B has an array `b` representing the atomic weight of each monomer.

Inside each chain, adjacent monomers are already connected by internal covalent bonds.

You must establish inter-chain cross-links connecting some monomers of Polymer A to some monomers of Polymer B.

The cost to create a link between monomer i of Polymer A and monomer j of Polymer B is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single monomer is removed (from either Polymer A or Polymer B).
If one monomer fails and disappears along with all its connections, the remaining monomers must still form a single connected network.

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
It's optimal to connect four pairs of monomers:
1. monomer 1 from Polymer A with monomer 2 from Polymer B: cost |1-4| = 3.
2. monomer 3 from Polymer A with monomer 2 from Polymer B: cost |1-4| = 3.
3. monomer 2 from Polymer A with monomer 1 from Polymer B: cost |10-20| = 10.
4. monomer 2 from Polymer A with monomer 3 from Polymer B: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first monomer of Polymer A with the first of Polymer B, and the last monomer of Polymer A with the last of Polymer B, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of monomers in each chain.
- The second line contains n integers representing the atomic weights of Polymer A.
- The third line contains n integers representing the atomic weights of Polymer B.

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
