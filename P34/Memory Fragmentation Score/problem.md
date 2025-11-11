## Title

Memory Fragmentation Score

## Slug

memory-fragmentation-score

## Difficulty

Medium

## Description

A computer system has $n$ memory blocks and $n$ processes, each ranked by size from 1 to $n$. When process $j$ is allocated to memory block $i$, it results in a "fragmentation score" of $i \times j$.A system architect is studying all $n^2$ possible allocations and needs to find the median fragmentation score. Given that $n$ is odd, calculate this value.

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