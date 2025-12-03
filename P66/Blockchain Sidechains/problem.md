## Title
Blockchain Sidechains

## Slug
blockchain-sidechains

## Difficulty
Medium

## Description
Two blockchains need bridges to swap assets securely even if a validator fails.

Two parallel chains, Mainnet and Sidenet, each contain n blocks arranged in a line.
Mainnet has an array `a` representing the hash difficulty of each block.
Sidenet has an array `b` representing the hash difficulty of each block.

Inside each chain, adjacent blocks are already connected by internal hashes.

You must establish inter-chain atomic swaps connecting some blocks of Mainnet to some blocks of Sidenet.

The cost to create a swap between block i of Mainnet and block j of Sidenet is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single block is removed (from either Mainnet or Sidenet).
If one block fails and disappears along with all its connections, the remaining blocks must still form a single connected network.

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
It's optimal to connect four pairs of blocks:
1. block 1 from Mainnet with block 2 from Sidenet: cost |1-4| = 3.
2. block 3 from Mainnet with block 2 from Sidenet: cost |1-4| = 3.
3. block 2 from Mainnet with block 1 from Sidenet: cost |10-20| = 10.
4. block 2 from Mainnet with block 3 from Sidenet: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first block of Mainnet with the first of Sidenet, and the last block of Mainnet with the last of Sidenet, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of blocks in each chain.
- The second line contains n integers representing the hash difficultys of Mainnet.
- The third line contains n integers representing the hash difficultys of Sidenet.

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
