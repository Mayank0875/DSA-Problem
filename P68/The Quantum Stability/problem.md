## Title
The Quantum Stability

## Slug
the-quantum-stability

## Difficulty
Hard

## Description
In a quantum computing lab, scientists are entangling qubits. There are n qubits, and some are already entangled links. The scientists believe that a quantum system is stable only if the number of qubits in an entangled cluster is a 'Stable Number'—a positive integer containing only the digits 4 and 7.

The lead researcher wants to stabilize the system by adding new entanglement links. Merging k existing clusters into one requires creating k - 1 new links.

Your task is to determine the minimum number of extra links the researcher needs to build to create at least one cluster whose size is a Stable Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect qubit 4 with qubit 3. We can also connect 4 with 1 or 2. This creates a cluster of size 4 (a Stable Number).

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
There is no way to connect the qubits to form a cluster with a size equal to a Stable Number.

## Input Format
- The first line contains two integers n and m: the number of qubits and the number of existing links.
- The next m lines each contain two integers u and v, representing a link between qubit u and qubit v. Note that u may be equal to v, and there may be multiple links connecting the same pair of qubits.

## Output Format
- Return a single integer: the minimum number of links to build. If no solution exists, print -1.

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
