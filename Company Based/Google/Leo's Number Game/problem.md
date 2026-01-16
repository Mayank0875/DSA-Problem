## Title

Leo's Number Game

## Slug

leos-number-game

## Difficulty

Medium

## Description

Leo is playing a mathematical card game. He starts with a score $k$ initially set to 0. The game consists of $n$ turns.

In each turn $i$, Leo is presented with two cards: a Red card with an integer $a_i$ and a Blue card with an integer $b_i$. He must choose exactly one card to play, which updates his score $k$ as follows:

* **Red Card:** The new score becomes $k - a_i$.
* **Blue Card:** The new score becomes $b_i - k$.

Leo plays optimally to maximize his final score after $n$ turns. Your task is to calculate the maximum score he can achieve.

## Examples

### 1

#### Input

3
4 -8 -1
-3 -7 0

#### Output

6

#### Explanation

Optimal path from note:
Turn 0: Blue (-3). Score: -3.
Turn 1: Red (-8). Score: $-3 - (-8) = 5$.
Turn 2: Red (-1). Score: $5 - (-1) = 6$.
    
### 2

#### Input

5
-3 1 0 7 1
-5 3 -1 4 -5

#### Output

12

#### Explanation

Optimal Score is 12.

## Input Format  

- The first line contains an integer $n$.
- The second line contains $n$ integers $a_1, a_2, \dots, a_n$ (Red card values).
- The third line contains $n$ integers $b_1, b_2, \dots, b_n$ (Blue card values).

## Output Format  

- Return a single integer representing the maximum possible score at the end of the game.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- -1e9 ≤ a_i, b_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, array, greedy