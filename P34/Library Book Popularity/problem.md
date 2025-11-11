## Title

Library Book Popularity

## Slug

library-book-popularity

## Difficulty

Medium

## Description

A library is organized into $n$ shelves, and each shelf has $n$ rows. Both shelves and rows are numbered 1 to $n$. The "popularity score" of the book at shelf $i$, row $j$ is $i \times j$.The librarian is doing an inventory and needs to find the median popularity score of all $n^2$ books. Given $n$ is an odd number, what is this value?

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