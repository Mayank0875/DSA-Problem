## Title

Assigning People to Lifeboats

## Slug

assigning-people-to-lifeboats

## Difficulty

Easy

## Description

During an emergency evacuation, people need to be assigned to lifeboats. Each lifeboat can carry one or two people. There is a maximum weight capacity, `x`, for each lifeboat. You are given the weights of `n` people waiting to board. To ensure safety and efficiency, you need to determine the minimum number of lifeboats required to save everyone, making sure no lifeboat exceeds its weight capacity.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One optimal assignment is:
    - Lifeboat 1: Person weighing 2 and person weighing 7 (Total weight 9 <= 10)
    - Lifeboat 2: Person weighing 3 (Total weight 3 <= 10)
    - Lifeboat 3: Person weighing 9 (Total weight 9 <= 10)
This requires 3 lifeboats.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One optimal assignment is:
    - Lifeboat 1: Person weighing 2 and person weighing 3 (Total weight 5 <= 5)
    - Lifeboat 2: Two people weighing 2 (Total weight 4 <= 5)
    - Lifeboat 3: Person weighing 4 (Total weight 4 <= 5)
This requires 3 lifeboats.

## Input Format

- The first line contains two integers n and x: the number of people and the maximum allowed weight per lifeboat.
- The second line contains n integers p_1, p_2, ..., p_n: the weight of each person.

## Output Format

- Return a single integer: the minimum number of lifeboats required.

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