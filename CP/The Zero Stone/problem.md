## Title

The Zero Stone

## Slug

the-zero-stone

## Difficulty

Easy

## Description

In the ancient ruins of Numeria, explorers found a magical artifact known as the Zero Stone. The stone currently holds a charge of energy represented by an integer $n$. To safely deactivate the stone and claim the treasure inside, the energy level must be reduced exactly to $0$.

The stone has a unique discharge mechanism: in a single step, you can reduce the current energy level by subtracting any one of the digits present in the number itself. For example, if the energy is $27$, you can subtract $2$ (becoming $25$) or $7$ (becoming $20$).

Your task is to determine the **minimum** number of steps required to reduce the energy of the Zero Stone from $n$ to $0$.

## Examples

### 1

#### Input

27

#### Output

5

#### Explanation

Total steps: 5.
    
### 2

#### Input

17

#### Output

3

#### Explanation

Total steps: 3.
  

## Input Format  

- The only input line has an integer n.

## Output Format  

- Return one integer: the minimum number of steps to reach 0.
  

## Constraints  

- 1 ≤ n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, maths