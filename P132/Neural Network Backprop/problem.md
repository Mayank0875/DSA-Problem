## Title
Neural Network Backprop

## Slug
neural-network-backprop

## Difficulty
Medium

## Description
An AI learns. Error signals must propagate back to the Input Layer.

There are $n$ neurons numbered from $1$ to $n$, connected by $n-1$ synapses. The network forms a tree structure (there is exactly one path between any two neurons). Currently, all synapses are one-way.

Learning algorithms route error to the **Input Layer (Node 1)**. To ensure success, every other neuron must be able to reach Input Layer by traveling along the synapses in the correct direction.

You are given the current orientation of the synapses. Your task is to determine the **minimum** number of synapses that need to be adjusted so that every neuron can reach Input Layer.

## Examples

### 1

#### Input
6
1 2
2 4
3 2
5 1
5 6

#### Output
3

#### Explanation
The destination is Input Layer (1).
- Synapse 1->2 points away from 1. Needs adjustment.
- Synapse 2->4 points away from 1. Needs adjustment.
- Synapse 3->2 points towards 2 (and effectively towards 1). OK.
- Synapse 5->1 points towards 1. OK.
- Synapse 5->6 points away from 1 (via 5). Needs adjustment.
Total adjustments: 3.

### 2

#### Input
5
2 1
2 3
4 3
4 5

#### Output
2

#### Explanation
Synapses 2->3 and 4->5 need to be adjusted.

## Input Format
- The first line contains an integer $n$ — the number of neurons.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way synapse from neuron $u$ to neuron $v$.

## Output Format
- Return a single integer representing the minimum number of synapses that need to be changed.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ u, v ≤ n
- The graph is guaranteed to be a tree.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
tree, depth-first-search, breadth-first-search, graph

## Company
google, amazon
