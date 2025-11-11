## Title

Signal Strength Grid

## Slug

signal-strength-grid

## Difficulty

Medium

## Description

A radio signal is being measured across an $n \times n$ (where $n$ is odd) grid. The coordinates $(i, j)$ range from 1 to $n$. The signal strength recorded at position $(i, j)$ is $i \times j$ due to interference patterns.A communications engineer needs to find the median signal strength from all $n^2$ measurements to determine the area's viability.

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