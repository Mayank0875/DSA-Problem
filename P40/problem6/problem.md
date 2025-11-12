## Title

Neural Fracture: Next Higher Synaptic Signal

## Slug

neural-fracture-next-higher-synaptic-signal

## Difficulty

Easy

## Description

A neuroscientist is examining a sequence of synaptic signal amplitudes recorded from a neural pathway to understand signal propagation patterns. For each recorded signal, they want to identify the amplitude of the nearest future signal that is strictly higher. This helps reveal potential amplification events or critical points in the neural cascade. If no future signal has a higher amplitude (either because it is the last measurement or all subsequent signals are lower or equal), this should be noted. Can you compute this for each signal in the sequence?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Signal 0 (500): Next higher is 600 (Signal 2). Output 600.  
Signal 1 (400): Next higher is 600 (Signal 2). Output 600.  
Signal 2 (600): Next higher is 700 (Signal 4). Output 700.  
Signal 3 (300): Next higher is 700 (Signal 4). Output 700.  
Signal 4 (700): Next higher is 800 (Signal 6). Output 800.  
Signal 5 (450): Next higher is 800 (Signal 6). Output 800.  
Signal 6 (800): No future signal is higher. Output -1.  
Signal 7 (500): No future signal exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All signal amplitudes are equal, so no future signal has a higher amplitude.

## Input Format

The first line contains a single integer n, the number of recorded signals.  
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the amplitude of each signal.

## Output Format

Return array of integers. The i‑th integer should be the amplitude of the nearest signal j > i such that a_j > a_i. If no such signal exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array