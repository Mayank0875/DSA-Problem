## Title

Sensor Array Readings

## Slug

sensor-array-readings

## Difficulty

Medium

## Description

An $n \times n$ square sensor array (where $n$ is odd) is deployed in a field to measure environmental data. Each sensor is identified by its coordinates $(i, j)$, where $i$ and $j$ range from 1 to $n$. The sensor at $(i, j)$ reports a value equal to $i \times j$.Scientists need to find the median sensor reading from all $n^2$ sensors to establish a baseline. Help them by finding this middle value.

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