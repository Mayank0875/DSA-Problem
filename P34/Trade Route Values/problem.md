## Title

Trade Route Values

## Slug

trade-route-values

## Difficulty

Medium

## Description

In a global trade simulation, there are $n$ import goods and $n$ export goods, each ranked in value from 1 to $n$. The "trade value" of pairing import good $i$ with export good $j$ is $i \times j$.Economists are studying the $n^2$ possible trade pairings and need to find the median trade value to assess the market. Given that $n$ is an odd integer, what is this value?

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