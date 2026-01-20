## Title

XOR Rivals

## Slug

xor-rivals

## Difficulty

Medium

## Description

Alex and Sam are playing a game with two binary arrays, $a$ and $b$, both of length $n$. The game consists of $n$ turns. Alex plays on odd-numbered turns (1st, 3rd, 5th...), and Sam plays on even-numbered turns (2nd, 4th, 6th...).

On the $i$-th turn, the current player can choose to either swap the elements $a_i$ and $b_i$, or do nothing. Note that a player can only modify the index corresponding to the current turn number.

At the end of the game, a score is calculated for each player. Alex's score is the bitwise XOR sum of all elements in array $a$. Sam's score is the bitwise XOR sum of all elements in array $b$. The player with the strictly higher score wins. If their scores are equal, the game is a Tie.

Assuming both Alex and Sam play optimally to win (or to tie if winning is impossible), determine the outcome of the game.

## Examples

### 1

#### Input

4
1 0 0 1
1 0 1 1

#### Output

Alex

#### Explanation

On turn 1, Alex swaps $a_1$ and $b_1$. Arrays become $a=[1,0,0,1]$, $b=[1,0,1,1]$.
On turn 2, Sam passes.
On turn 3, Alex swaps. Arrays become $a=[1,0,1,1]$, $b=[1,0,0,1]$.
On turn 4, Sam swaps. Arrays become $a=[1,0,1,1]$, $b=[1,0,0,1]$.
Final XOR sums: Alex = $1 \oplus 0 \oplus 1 \oplus 1 = 1$, Sam = $1 \oplus 0 \oplus 0 \oplus 1 = 0$. Alex wins.
    
### 2

#### Input

4
0 0 1 0
1 0 1 1

#### Output

Tie

#### Explanation

With optimal play, neither player can force a win.  

## Input Format  

- The first line contains an integer $n$, the size of the arrays.
- The second line contains $n$ integers representing array $a$.
- The third line contains $n$ integers representing array $b$.

## Output Format  

- Return "Alex" if Alex wins, "Sam" if Sam wins, or "Tie" if it is a tie.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 0 ≤ a[i], b[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, greedy, math

## Company
google