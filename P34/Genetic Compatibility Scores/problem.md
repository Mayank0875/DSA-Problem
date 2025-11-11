## Title

Genetic Compatibility Scores

## Slug

genetic-compatibility-scores

## Difficulty

Medium

## Description

Geneticists are studying the compatibility between $n$ genes from Species A (labeled 1 to $n$) and $n$ genes from Species B (labeled 1 to $n$). The compatibility score for pairing gene $i$ from Species A with gene $j$ from Species B is calculated as $i \times j$.To understand the overall compatibility, find the median score among all $n^2$ possible pairings. You are given that $n$ is an odd integer.

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