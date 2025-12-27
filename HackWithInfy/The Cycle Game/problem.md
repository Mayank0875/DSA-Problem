## Title

The Cycle Game

## Slug

the-cycle-game

## Difficulty

Hard

## Description

Obada and Harraaak are two grandmasters playing a strategic game using a permutation p of length n. The game starts with a score of 0.

The players take turns, with Obada moving first. On each turn, a player chooses an integer x from the permutation that has not been chosen before.
If it is Obada’s turn, the chosen value x is added to the score.
If it is Harraaak’s turn, the chosen value x is subtracted from the score.

The rules for choosing x are:

On the very first move of the game, Obada may choose any unselected element from the permutation.
On every move after the first:

Let m be the index of the element chosen in the previous move (that is, the previous player chose p[m]).

If the value p[m] has not yet been chosen, the current player must choose p[m].
If p[m] has already been chosen, the current player may choose any unselected element.

The game continues until all elements of the permutation have been chosen.

Obada plays optimally to maximize the final score, while Harraaak plays optimally to minimize it.

Your task is to compute the final score assuming both players play optimally.

## Examples

### 1

#### Input

3
2 3 1

#### Output

4

#### Explanation

Obada chooses numbers to add, Harraaak chooses numbers to subtract.
By choosing the best possible starting number and playing optimally, Obada can achieve a maximum final score of 4.

    
### 2

#### Input

2
2 1

#### Output

1

#### Explanation

Obada chooses 2 and adds it to the score.
Harraaak then subtracts 1, the only remaining number.
Final score is 1.
  

## Input Format  

- First line contains an integer n (length of permutation).
- n space-separated integers p_1, ....., p_n.

## Output Format  

- Return one integer: final score.
  

## Constraints  

- 1 ≤ n ≤ 1e6
- 1 ≤ p_i ≤ n

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

greedy, graph, combinatrics , hackwithinfy

## Companies
infosys
