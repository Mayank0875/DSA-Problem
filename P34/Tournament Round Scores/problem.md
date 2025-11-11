## Title

Tournament Round Scores

## Slug

tournament-round-scores

## Difficulty

Medium

## Description

In a special tournament, $n$ teams (numbered 1 to $n$) play in $n$ rounds (numbered 1 to $n$). The score a team gets is based on their skill and the round number. Specifically, team $i$ in round $j$ receives a score of $i \times j$.The tournament organizer wants to find the median score from all $n^2$ scores (one for each team in each round) to analyze the game's balance. Given $n$ is odd, find the median score.

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