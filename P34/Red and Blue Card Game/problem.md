## Title

Red and Blue Card Game

## Slug

red-blue-card-game

## Difficulty

Medium

## Description

In a card game, you have two decks: a red deck and a blue deck. Each deck contains $n$ cards, with values from 1 to $n$. You draw one red card (with value $i$) and one blue card (with value $j$). Your score for the round is $i \times j$.You want to find the median score possible across all $n^2$ combinations of red and blue cards. Given that $n$ is an odd number, find this value.

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