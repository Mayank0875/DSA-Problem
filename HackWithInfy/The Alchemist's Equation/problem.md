## Title

The Alchemist's Equation

## Slug

the-alchemists-equation

## Difficulty

Medium

## Description

In the ancient laboratory of Alexandria, a legendary alchemist left behind a riddle involving a collection of rare elements. Each element possesses a specific atomic energy value. The alchemist claimed that the key to the Philosopher's Stone lies in combining a subset of these elements such that their total energy sums up to a precise target value, $X$.

You are given a list of $n$ elements, where the $i$-th element has an energy value $t_i$. Your task is to determine the number of distinct subsets of these elements whose sum of energy values equals exactly $X$.

The order of elements in a subset does not matter, but distinct elements with the same energy value are considered different entities (i.e., we are looking for the number of ways to choose indices).

## Examples

### 1

#### Input

4 5
1 2 3 2

#### Output

3

#### Explanation

Total ways: 3.
    
### 2

#### Input

2 10
5 6

#### Output

0

#### Explanation

Possible sums are 0 (empty set), 5, 6, and 11. None equal 10.

## Input Format  

- The first line contains two integers n and X: the number of elements and the target energy sum.
- The second line contains $n$ integers $t_1, t_2, \dots, t_n$: the energy values of the elements.

## Output Format  

- Return one integer: the number of ways to create a subset with sum exactly X.
  

## Constraints  

- 1 ≤ n ≤ 40
- 1 ≤ x ≤ 1e9
- 1 ≤ t_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, breadth-first-search, divide-and-conquer, hackwithinfy

## Companies
infosys