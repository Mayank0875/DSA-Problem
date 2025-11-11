## Title

Recipe Flavor Rating

## Slug

recipe-flavor-rating

## Difficulty

Medium

## Description

A chef is experimenting with $n$ different spices and $n$ different main ingredients, each ranked from 1 to $n$. The "flavor rating" of combining spice $i$ with ingredient $j$ is $i \times j$.The chef wants to find the median flavor rating from all $n^2$ combinations to create a new menu. Given that $n$ is an odd integer, find this median.

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