## Title
Neural Network Pulse

## Slug
neural-network-pulse

## Difficulty
Medium

## Description
A signal fires from Input Neuron (node 1) to Output Neuron (node n).

The brain has `n` neurons and `m` directed synapses. Synapses may repeat between the same pair of neurons and self-loops are allowed. A firing pattern of length `k` is a sequence of exactly `k` directed synapses; neurons and synapses may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed synapses (each synapse given as two integers `u` `v` meaning a directed synapse from `u` to `v`), compute the number of distinct firing patterns that start at neuron 1 and end at neuron `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 neurons. We want the number of directed firing patterns of length 8 from neuron 1 to neuron 3.
Valid length-8 firing patterns:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such firing patterns.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has synapses 1->2 and 2->3, the only firing pattern of length 2 from neuron 1 to neuron 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of neurons, synapses, and the required firing pattern length.
- The next m lines describe the synapses. Each line contains two integers u and v, indicating a directed synapse from neuron u to neuron v.

## Output Format
- Return single integer: the number of firing patterns modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
