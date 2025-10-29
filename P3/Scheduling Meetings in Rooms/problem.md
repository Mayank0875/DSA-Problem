## Title

Scheduling Meetings in Rooms

## Slug

scheduling-meetings-rooms

## Difficulty

Easy

## Description

You are scheduling meetings in conference rooms. Each room can host one or two meetings during a specific time block (assume all meetings fit within this block if scheduled). The constraint is that the total duration of meeting(s) scheduled in one room for this block cannot exceed `x` hours. You have `n` meetings, each with a known duration. What is the minimum number of conference rooms needed to schedule all meetings for this block?

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One minimal room usage:
    - Room 1: Meeting of 2 hours and meeting of 7 hours (Total duration 9 <= 10)
    - Room 2: Meeting of 3 hours (Total duration 3 <= 10)
    - Room 3: Meeting of 9 hours (Total duration 9 <= 10)
This requires 3 rooms.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One minimal room usage:
    - Room 1: Meeting of 2 hours and meeting of 3 hours (Total duration 5 <= 5)
    - Room 2: Two meetings of 2 hours (Total duration 4 <= 5)
    - Room 3: Meeting of 4 hours (Total duration 4 <= 5)
This requires 3 rooms.

## Input Format

- The first line contains two integers n and x: the number of meetings and the maximum total duration per room (in hours).
- The second line contains n integers p_1, p_2, ..., p_n: the duration of each meeting (in hours).

## Output Format

- Return a single integer: the minimum number of rooms required.

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