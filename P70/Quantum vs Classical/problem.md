## Title
Quantum vs Classical

## Slug
quantum-vs-classical

## Difficulty
Medium

## Description
Quantum bits Tunnel. Classical bits flow through Wires. Wires connect gates that don't allow Tunneling.

The processor has n gates numbered from 1 to n.
The Tunneling connects specific pairs of gates with direct tunnels.
The Wiring is constructed based on a unique rule:
A direct wire exists between two gates if and only if there is no tunnel connecting them.

Moving between any two connected gates takes exactly 1 hour on either network.
Two bits, Q-Bit and C-Bit, depart from gate 1 at the same time, heading for gate n.

1. Q-Bit travels only using Tunneling.
2. C-Bit travels only using Wiring.

To ensure safety, they must never arrive at the same gate at the same time (except for the final gate n).
Your task is to compute the minimum number of hours required for **both** bits to reach gate n — specifically, the time when the slower bit arrives.
If either bit cannot reach gate n using their respective network, return -1.

## Examples

### 1

#### Input
4 2
1 3
3 4

#### Output
2

#### Explanation
The smallest possible time is 2. One takes the direct route (1 hour), the other takes a path of length 2.

### 2

#### Input
4 6
1 2
1 3
1 4
2 3
2 4
3 4

#### Output
-1

#### Explanation
The graph is fully connected for one network, meaning the complement network has no edges. The second bit cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of gates and the number of tunnels.
- The next m lines each contain two integers u and v, representing a tunnel between gates u and v.
- The graph is bidirectional. There is at most one tunnel between any pair of gates.

## Output Format
- Return a single integer representing the minimum hours required for the last bit to arrive. If it is impossible, return -1.

## Constraints
- 2 ≤ n ≤ 400
- 0 ≤ m ≤ n(n - 1)/2
- 1 ≤ u, v ≤ n
- u ≠ v

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
