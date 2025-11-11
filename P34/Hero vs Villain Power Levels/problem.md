## Title

Hero vs Villain Power Levels

## Slug

hero-villain-power-levels

## Difficulty

Medium

## Description

In a new superhero simulator, $n$ heroes (ranked 1 to $n$) are pitted against $n$ villains (ranked 1 to $n$). When hero $i$ fights villain $j$, the power level of the battle is $i \times j$.The game designer needs to analyze the balance of all $n^2$ possible matchups. Find the median power level of all fights. It is given that $n$ is an odd integer.

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