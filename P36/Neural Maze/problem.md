## Title

Neural Maze

## Slug

neural-maze

## Difficulty

Medium

## Description

A neuroscientist arranges n artificial neurons in a straight line, numbered 1 to n. Initially, all neurons are firing.
The scientist sends n pulses. For the i‑th pulse (where i goes from 1 to n), every neuron whose number j is a multiple of i toggles its state. 
A firing neuron becomes silent, and a silent neuron becomes firing. After all n pulses are sent, the scientist observes the final state of the neurons. The scientist needs exactly k neurons to be firing in the end. Find the smallest possible number of neurons n the scientist should start with to achieve exactly k firing neurons.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [F]. Pulse 1 toggles 1: [S]. Final: 0 firing.
If n=2, initial: [F, F]. Pulse 1 toggles 1, 2: [S, S]. Pulse 2 toggles 2: [S, F]. Final: 1 firing (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [F,F,F,F,F].
Pulse 1 toggles 1,2,3,4,5 -> [S,S,S,S,S].
Pulse 2 toggles 2,4 -> [S,F,S,F,S].
Pulse 3 toggles 3 -> [S,F,F,F,S].
Pulse 4 toggles 4 -> [S,F,F,S,S].
Pulse 5 toggles 5 -> [S,F,F,S,F].
Final state: 3 neurons (2, 3, 5) are firing (k=3). We can show n=4 results in only 2 firing neurons ([S,F,F,S]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of neurons required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory