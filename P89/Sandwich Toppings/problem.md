## Title
Sandwich Toppings

## Slug
sandwich-toppings

## Difficulty
Medium

## Description
Chefs remove toppings from a sub sandwich.

The game involves toppings numbered $1, 2, \dots, n$.
The game is played in turns, and Chef 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining toppings.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left topping or the right topping from the sequence. The game then continues with the other player.

Both Chef 1 and Chef 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of toppings $n$.

## Examples

### 1

#### Input
1

#### Output
Chef 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Chef 1 removes 1. The remaining sequence is empty (XOR sum 0). Chef 2 cannot move and loses. Chef 1 wins.

### 2

#### Input
2

#### Output
Chef 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Chef 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Chef 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Chef 1 to lose on the next turn. Chef 2 wins.

## Input Format
- The only input line has an integer n, the number of toppings.

## Output Format
- Return "Chef 1" if Chef 1 wins, or "Chef 2" if Chef 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
