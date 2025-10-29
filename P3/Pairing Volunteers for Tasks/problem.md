## Title

Pairing Volunteers for Tasks

## Slug

pairing-volunteers-tasks

## Difficulty

Easy

## Description

An event organizer is assigning volunteers to tasks. Each task requires either one or two volunteers. The combined 'skill level' (represented numerically, lower means less demanding) needed for a task cannot exceed a maximum value `x`. You have `n` volunteers, each with a specific skill level rating. What is the minimum number of tasks needed to assign all volunteers, either individually or in pairs, ensuring the skill level limit for each task is met?

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One minimal task assignment:
    - Task 1: Volunteer level 2 and volunteer level 7 (Total skill 9 <= 10)
    - Task 2: Volunteer level 3 (Total skill 3 <= 10)
    - Task 3: Volunteer level 9 (Total skill 9 <= 10)
This requires 3 tasks.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One minimal task assignment:
    - Task 1: Volunteer level 2 and volunteer level 3 (Total skill 5 <= 5)
    - Task 2: Two volunteers level 2 (Total skill 4 <= 5)
    - Task 3: Volunteer level 4 (Total skill 4 <= 5)
This requires 3 tasks.

## Input Format

- The first line contains two integers n and x: the number of volunteers and the maximum combined skill level per task.
- The second line contains n integers p_1, p_2, ..., p_n: the skill level of each volunteer.

## Output Format

- Return a single integer: the minimum number of tasks required.

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