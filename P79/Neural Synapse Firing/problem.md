## Title
Neural Synapse Firing

## Slug
neural-synapse-firing

## Difficulty
Medium

## Description
Neurons transmit impulses. Synapses enter a refractory period (blocked) after firing once.

The brain consists of $n$ neurons and $m$ one-way axons. Each axon connects a specific source neuron to a destination neuron.

The process happens over several impulses. In each impulse, you must send a impulse from neuron 1 (the source) to neuron $n$ (the destination). The catch is that each axon becomes temporarily inactive (refractory) after firing. This means each axon can be used at most once across all impulses combined.

Your goal is to determine the maximum number of impulses you can successfully complete the journey from neuron 1 to neuron $n$.

## Examples

### 1

#### Input
6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output
2

#### Explanation
You can complete 2 impulses.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 impulse.

## Input Format
- The first line contains two integers $n$ and $m$: the number of neurons and the number of axons.
- The next $m$ lines describe the axons. Each line contains two integers $a$ and $b$, indicating a directed axon from neuron $a$ to neuron $b$.

## Output Format
- Return one integer: the maximum number of impulses possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
