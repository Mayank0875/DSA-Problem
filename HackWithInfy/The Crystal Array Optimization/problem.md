## Title

The Crystal Array Optimization

## Slug

the-crystal-array-optimization

## Difficulty

Hard

## Description

In the high-tech city of Bitopolis, engineers are working on a new energy storage system using a linear array of n power crystals.

Each crystal must store a positive integer amount of energy, and the total energy stored across all crystals must be exactly k.

However, placing crystals with certain energy levels next to each other causes interference. The interference cost between two adjacent crystals with energy values x and y is defined as:

x & y (bitwise AND)

The total interference cost of the system is the sum of the interference costs between all adjacent pairs in the array:
For i from 2 to n:
add (a[i] & a[i-1]) to the cost

Your task is to determine the minimum possible interference cost that can be achieved by choosing appropriate energy levels for the array of size n such that the sum of all elements is exactly k.

## Examples

### 1

#### Input

2 4

#### Output

1

#### Explanation

For n = 2 and k = 4, possible arrays are [1, 3] with cost 1 and [2, 2] with cost 2, so the minimum cost is 1.
Since 4 is a power of two, it cannot be split into two numbers with completely disjoint bits, which fixes the optimal answer at 1.
    
### 2

#### Input

2 5

#### Output

0

#### Explanation

We can choose array $[4, 1]$. Sum is 5. Cost is $4 \ \& \ 1 = 0$.

  

## Input Format  

- The only input line has two space-separated integers $n$ and $k$.

## Output Format  

- Return one integer: representing the minimum cost.
  

## Constraints  

- 1 ≤ n ≤ 1e6
- n ≤ k ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

maths, greedy, hackwithinfy

## Companies
infosys