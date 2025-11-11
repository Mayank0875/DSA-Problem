## Title

Racing Game Lap Times

## Slug

racing-game-lap-times

## Difficulty

Medium

## Description

In a new racing video game, there are $n$ cars (ranked 1 to $n$) and $n$ tracks (ranked 1 to $n$). The physics engine determines that the lap time for car $i$ on track $j$ is $i \times j$ seconds.The developers need to find the median lap time among all $n^2$ car-track combinations to balance the game. Given $n$ is an odd number, what is the median time?

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