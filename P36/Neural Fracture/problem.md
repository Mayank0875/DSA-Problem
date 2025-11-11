## Title

Neural Fracture

## Slug

neural-fracture

## Difficulty

Medium

## Description

A neuroscientist models a linear chain of *n* neurons, numbered 1 to *n*. Initially, every neuron is firing (active).  
The scientist applies *n* stimulation rounds. In the *i*‑th round (for *i* = 1 to *n*), every neuron whose index *j* is a multiple of *i* toggles its state: an active neuron becomes inactive, and an inactive neuron becomes active.  
After all *n* rounds, the scientist observes the final pattern of activity. She needs exactly *k* neurons to be active at the end. Determine the smallest possible size *n* of the chain that yields exactly *k* active neurons.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [A]. Round 1 toggles 1: [I]. Final: 0 active.  
If n=2, initial: [A, A]. Round 1 toggles 1, 2: [I, I]. Round 2 toggles 2: [I, A]. Final: 1 active (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [A,A,A,A,A].  
Round 1 toggles 1,2,3,4,5 → [I,I,I,I,I].  
Round 2 toggles 2,4 → [I,A,I,A,I].  
Round 3 toggles 3 → [I,A,A,A,I].  
Round 4 toggles 4 → [I,A,A,I,I].  
Round 5 toggles 5 → [I,A,A,I,A].  
Final state: 3 neurons (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active neurons ([I,A,A,I]), so 5 is the minimum.
  

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