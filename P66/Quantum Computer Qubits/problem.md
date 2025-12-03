## Title
Quantum Computer Qubits

## Slug
quantum-computer-qubits

## Difficulty
Medium

## Description
Two registers of qubits need entanglement links to maintain coherence despite errors.

Two parallel registers, Register X and Register Y, each contain n qubits arranged in a line.
Register X has an array `a` representing the energy state of each qubit.
Register Y has an array `b` representing the energy state of each qubit.

Inside each register, adjacent qubits are already connected by internal couplings.

You must establish inter-register entanglement links connecting some qubits of Register X to some qubits of Register Y.

The cost to create a link between qubit i of Register X and qubit j of Register Y is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single qubit is removed (from either Register X or Register Y).
If one qubit fails and disappears along with all its connections, the remaining qubits must still form a single connected network.

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
It's optimal to connect four pairs of qubits:
1. qubit 1 from Register X with qubit 2 from Register Y: cost |1-4| = 3.
2. qubit 3 from Register X with qubit 2 from Register Y: cost |1-4| = 3.
3. qubit 2 from Register X with qubit 1 from Register Y: cost |10-20| = 10.
4. qubit 2 from Register X with qubit 3 from Register Y: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first qubit of Register X with the first of Register Y, and the last qubit of Register X with the last of Register Y, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of qubits in each register.
- The second line contains n integers representing the energy states of Register X.
- The third line contains n integers representing the energy states of Register Y.

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
