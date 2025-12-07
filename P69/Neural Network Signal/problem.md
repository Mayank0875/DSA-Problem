## Title
Neural Network Signal

## Slug
neural-network-signal

## Difficulty
Hard

## Description
A signal propagates from input neurons to output neurons. The synaptic weights effectively limit the 'strength' that can pass.

The network consists of n neurons, numbered 1 to n.
1. Neuron 1 is the Input Layer.
2. Neuron n is the Output Layer.

There are m one-way axons connecting these neurons. Each axon has a specific capacity, measured in signal units, which limits the rate at which impulses can flow through it.

Multiple axons can exist between the same two neurons, and their capacities stack. Your goal is to determine the maximum total signal strength that can be achieved from the Input Layer to the Output Layer using the available network.

## Examples

### 1

#### Input
4 5
1 2 3
2 4 2
1 3 4
3 4 5
4 1 3

#### Output
6

#### Explanation
There are two main paths to transmit impulses from node 1 to node 4:
1 -> 2 -> 4 (capacity limited by link 2 -> 4 with capacity 2).
1 -> 3 -> 4 (capacity limited by link 1 -> 3 with capacity 4).
Total max flow is 2 + 4 = 6. The link 4 -> 1 is ignored because it flows backward from the destination.

### 2

#### Input
3 2
1 2 5
2 3 5

#### Output
5

#### Explanation
A single path 1 -> 2 -> 3 exists with a bottleneck capacity of 5.

## Input Format
- The first line contains two integers n and m: the number of neurons and the number of axons.
- The next m lines describe the axons. Each line contains three integers u, v, and c, indicating a one-way axon from Neuron u to Neuron v with capacity c.

## Output Format
- Return one integer: the maximum signal strength from Neuron 1 to Neuron n.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ u, v ≤ n
- 1 ≤ c ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
