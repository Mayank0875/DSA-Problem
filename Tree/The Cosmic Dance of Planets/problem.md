## Title

The Cosmic Dance of Planets

## Slug

cosmic-dance-of-planets

## Difficulty

Easy

## Description

In a distant galaxy, $n$ mystical planets are arranged in a straight line, numbered from $1$ to $n$. Every millennium, a cosmic event occurs where the planets change their positions simultaneously based on a fixed divine law. This law is defined by a permutation $p$, where the planet currently at position $i$ moves to the new position $p_i$.The Great Astronomer wants to know how many millenniums must pass for all planets to return to their original starting positions $(1, 2, \dots, n)$ for the first time. Since the universe is vast and the number of millenniums can be very large, you must calculate the result modulo $10^9 + 7$. Can you help the Astronomer determine the duration of this cosmic cycle?

## Examples

### 1

#### Input

3
2 3 1

#### Output

3

#### Explanation

Initial State: [1, 2, 3]
After 1 millennium: Position 1 moves to 2, 2 to 3, 3 to 1. State: [3, 1, 2]
After 2 millenniums: State: [2, 3, 1]
After 3 millenniums: State: [1, 2, 3]
All planets are back to their original positions.
    
### 2

#### Input

8
5 3 2 6 4 1 8 7

#### Output

4

#### Explanation

It can be proven there will no way to do in less than 4 ways.

## Input Format  

- The first line has an integer n.
- The second line of contains $n$ integers, $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$). It is guaranteed that all $p_i$ are distinct.

## Output Format  

Return a single integer representing the number of millenniums required modulo $10^9 + 7$.
  

## Constraints  

- 1 ≤ n ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, graph, Maths

## Company
google