## Title

Assigning Animals to Enclosures

## Slug

assigning-animals-enclosures

## Difficulty

Easy

## Description

A zoo is assigning animals to temporary enclosures. Each enclosure can house one or two animals. For compatibility reasons, the total 'space requirement' (represented numerically) of the animal(s) in one enclosure cannot exceed a limit `x`. You are given the space requirements for `n` animals. Determine the minimum number of enclosures needed to house all animals while respecting the space limit per enclosure.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One efficient assignment:
    - Enclosure 1: Animal needing 2 units and animal needing 7 units (Total space 9 <= 10)
    - Enclosure 2: Animal needing 3 units (Total space 3 <= 10)
    - Enclosure 3: Animal needing 9 units (Total space 9 <= 10)
This requires 3 enclosures.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One efficient assignment:
    - Enclosure 1: Animal needing 2 units and animal needing 3 units (Total space 5 <= 5)
    - Enclosure 2: Two animals needing 2 units (Total space 4 <= 5)
    - Enclosure 3: Animal needing 4 units (Total space 4 <= 5)
This requires 3 enclosures.

## Input Format

- The first line contains two integers n and x: the number of animals and the maximum space requirement per enclosure.
- The second line contains n integers p_1, p_2, ..., p_n: the space requirement of each animal.

## Output Format

- Return a single integer: the minimum number of enclosures required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers