## Title
Neural Network Pruning

## Slug
neural-network-pruning

## Difficulty
Medium

## Description
Neurons are connected in a tree. The brain prunes connections by strengthening pairs of firing neurons. Each neuron strengthens a link with one neighbor.

The structure is a tree with n neurons and n-1 synapses.
A strengthened link is formed between two neurons connected by a synapse.
However, each neuron can be part of at most one strengthened link.

Your task is to calculate the maximum number of strengthened links that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of strengthened links is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 strengthened links.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form strengthened links (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of neurons.
- The next n-1 lines each contain two integers u and v, representing a synapse between neuron u and neuron v.

## Output Format
- Return a single integer representing the maximum number of strengthened links.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
