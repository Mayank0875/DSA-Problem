## Title

Radio Signal Clarity

## Slug

radio-signal-clarity

## Difficulty

Medium

## Description

A communications array has $n$ transmitters and $n$ receivers, each ranked from 1 to $n$. The "signal clarity" when pairing transmitter $i$ with receiver $j$ is calculated as $i \times j$.An engineer is studying all $n^2$ pairings to find the median signal clarity. Given $n$ is an odd number, find this value.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The numbers in increasing order are [1,2,2,3,3,4,6,6,9], so the answer is 3. 
    
### 2

#### Input

5

#### Output

8

#### Explanation
The middle element is 8.
  

## Input Format  

- The only input line has an integer n.

## Output Format  

- Return one integer: the answer to the task.
  

## Constraints  

- 1 ≤ x ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory