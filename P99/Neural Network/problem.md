## Title
Neural Network

## Slug
neural-network

## Difficulty
Hard

## Description
AI researchers activate neurons. Synapses fire to specific next neurons.

Researcher and Glitch are playing a strategic game using a neuron layer $p$ of length $n$. The game starts with a activation sum of 0.

The players take turns, with Researcher moving first. On each turn, a player chooses an integer $x$ from the neuron layer that has not been chosen before.
- If it is Researcher's turn, the chosen value $x$ is **added** to the activation sum.
- If it is Glitch's turn, the chosen value $x$ is **subtracted** from the activation sum.

The rules for choosing $x$ are:
1. On the very first move of the game, Researcher may choose **any** unselected neuron from the neuron layer.
2. On every move after the first:
   - Let $m$ be the index of the neuron chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected neuron.

The game continues until all neurons of the neuron layer have been chosen.

Researcher plays optimally to **maximize** the final activation sum, while Glitch plays optimally to **minimize** it.

Your task is to compute the final activation sum assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final activation sum is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final activation sum is 1.

## Input Format
- The first line contains an integer $n$ (length of neuron layer).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final activation sum on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
