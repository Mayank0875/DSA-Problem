## Title

Alien Artifact Grid

## Slug

alien-artifact-grid

## Difficulty

Medium

## Description

Archaeologists have discovered an $n \times n$ (where $n$ is odd) grid of alien artifacts. The artifacts are located at positions $(i, j)$ with $i$ and $j$ from 1 to $n$. The energy signature of the artifact at $(i, j)$ is measured to be $i \times j$.To classify the site, scientists need to find the median energy signature among all $n^2$ artifacts.

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