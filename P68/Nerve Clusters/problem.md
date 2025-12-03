## Title
Nerve Clusters

## Slug
nerve-clusters

## Difficulty
Hard

## Description
n neurons are in a brain scan. Synapses connect some into clusters. The AI seeks clusters of 'Thought Size' (digits 4 and 7).

You can simulate synapses. Merging k clusters costs k - 1 simulations.

Your task is to determine the minimum number of extra simulations the AI needs to build to create at least one cluster whose size is a Thought Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect neuron 4 with neuron 3. We can also connect 4 with 1 or 2. This creates a cluster of size 4 (a Thought Size).

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
There is no way to connect the neurons to form a cluster with a size equal to a Thought Size.

## Input Format
- The first line contains two integers n and m: the number of neurons and the number of existing simulations.
- The next m lines each contain two integers u and v, representing a synapse between neuron u and neuron v. Note that u may be equal to v, and there may be multiple simulations connecting the same pair of neurons.

## Output Format
- Return a single integer: the minimum number of simulations to build. If no solution exists, print -1.

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
