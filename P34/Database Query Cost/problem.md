## Title

Database Query Cost

## Slug

database-query-cost

## Difficulty

Medium

## Description

A database administrator is analyzing query performance. The system has $n$ tables (ranked 1 to $n$) and $n$ query types (ranked 1 to $n$). The "cost" of running query type $j$ on table $i$ is $i \times j$ units.To optimize the database, the DBA needs to find the median query cost from all $n^2$ possible query-table pairs. Given $n$ is an odd integer, find this median.

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