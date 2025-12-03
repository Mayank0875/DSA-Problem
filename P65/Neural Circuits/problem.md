## Title
Neural Circuits

## Slug
neural-circuits

## Difficulty
Medium

## Description
Neurons fire signals to other neurons. A Neural Circuit is a group of neurons that can sustain a signal loop.

Two neurons a and b belong to the same Neural Circuit if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of synapses.
In other words, two neurons are in the same Neural Circuit if they are mutually reachable.

Your task is to: Determine how many Neural Circuits exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The neurons form two distinct groups where round-trip traversal is possible within each group.
Neurons {1, 2, 3} form one Neural Circuit.
Path: 1 -> 2 -> 3 -> 1.
Neurons {4, 5} form another Neural Circuit.
Path: 4 -> 5 -> 4.
Total Neural Circuits: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 neurons and 1 one-way synapse.
Synapse: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Neural Circuits.

## Input Format
- The first line contains two integers n and m: the number of neurons and synapses.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way synapse from neuron a to neuron b.

## Output Format
- Return one integer: the total number of Neural Circuits.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, strongly-connected-components
