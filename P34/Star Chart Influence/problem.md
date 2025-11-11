## Title

Star Chart Influence

## Slug

star-chart-influence

## Difficulty

Medium

## Description

An ancient star chart is represented as an $n \times n$ grid ($n$ is odd). The rows and columns are indexed from 1 to $n$. The "celestial influence" of the sector at coordinates $(i, j)$ is calculated as $i \times j$.An astrologer wants to find the median celestial influence from all $n^2$ sectors to make a prediction. Find this median value.

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