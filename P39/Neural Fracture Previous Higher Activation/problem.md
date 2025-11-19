## Title

Neural Fracture: Previous Higher Activation

## Slug

neural-fracture-previous-higher-activation

## Difficulty

Easy

## Description

Imagine traversing a chain of neurons, each emitting a signal of varying strength. As you examine each neuron, you look back (to the earlier neurons) and want to know the strength of the nearest neuron that emitted a strictly stronger signal than the current one. If all previous neurons emitted weaker or equal signals, or if it's the first neuron, there is no such stronger predecessor. Your goal is to determine this stronger signal's strength for each position in the chain.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Neuron 0 (30): No previous neuron. Output -1.
Neuron 1 (60): Neuron 0 (30) is weaker. Output -1.
Neuron 2 (90): Neurons 0 (30), 1 (60) are weaker. Output -1.
Neuron 3 (50): Neuron 2 (90) is the nearest stronger. Output 90.
Neuron 4 (80): Neuron 2 (90) is the nearest stronger. Output 90.
Neuron 5 (40): Neuron 4 (80) is the nearest stronger. Output 80.
Neuron 6 (70): Neuron 4 (80) is the nearest stronger. Output 80.
Neuron 7 (50): Neuron 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All neurons emit equal signals, so no strictly stronger previous neuron exists.

## Input Format

The first line contains a single integer n, the number of neurons.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the signal strength of each neuron.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest neuron j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array