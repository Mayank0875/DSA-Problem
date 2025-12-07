## Title
Blockchain Fraud

## Slug
blockchain-fraud

## Difficulty
Medium

## Description
Forensics analyze crypto transactions. Wash trading involves sending money in circles to fake volume.

A "wash loop" occurs when funds moves from a wallet, through a sequence of transfers, and returns to the starting wallet without traversing the same transfer twice in immediate succession. The "length" of such a wash loop is the number of transfers it contains.

Detect the tightest wash trading circle. Find the number of transfers in the shortest loop.

Given the layout of the ledger, determine the length of the shortest wash loop.

## Examples

### 1

#### Input
5 6
1 2
1 3
2 4
2 5
3 4
4 5

#### Output
3

#### Explanation
There are several wash loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest wash loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no wash loops in this network.

## Input Format
- The first line contains two integers n and m: the number of wallets and the number of transfers.
- The wallets are numbered 1, 2, ..., n.
- The next m lines describe the transfers. Each line contains two integers u and v, indicating a connection between wallet u and wallet v.
- The graph is undirected. There is at most one transfer between any two wallets.

## Output Format
- Return one integer: the length of the shortest wash loop. If there are no wash loops, print `-1`.

## Constraints
- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
