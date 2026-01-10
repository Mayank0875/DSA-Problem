## Title
Network Node Ping

## Slug
network-node-ping

## Difficulty
Medium

## Description
Nodes 1 to n respond to pings. The network 'mesh' is established from the root if nodes 1 to k have responded.

There is a sequence of $n$ nodes indexed from $1$ to $n$. Initially, all nodes are **waiting**.

You ping the nodes one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you ping the node at the position `sequence[i-1]`.

A state is called **established** if, after performing $k$ steps, exactly the first $k$ nodes (indices $1$ to $k$) are active and all other nodes are waiting.

Your task is to calculate how many times the system becomes **established** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not established)
- Step 2 (index 2): "01100" (Not established)
- Step 3 (index 4): "01110" (Not established)
- Step 4 (index 1): "11110" (established: first 4 are active)
- Step 5 (index 5): "11111" (established: first 5 are active)
Total established states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not established)
- Step 2 (index 1): "1001" (Not established)
- Step 3 (index 2): "1101" (Not established)
- Step 4 (index 3): "1111" (established)
Total established states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was established.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
