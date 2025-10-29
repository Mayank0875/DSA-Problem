## Title

Forming Student Project Teams

## Slug

forming-student-project-teams

## Difficulty

Easy

## Description

A professor needs to assign students to project teams. Each team can have either one or two students. To ensure balanced effort, the total estimated 'effort points' (represented by weights) for the students in a single team cannot exceed a maximum value `x`. Given the estimated effort points for `n` students, what is the minimum number of teams the professor needs to form to include all students?

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One way to form minimal teams:
    - Team 1: Student with 2 points and student with 7 points (Total effort 9 <= 10)
    - Team 2: Student with 3 points (Total effort 3 <= 10)
    - Team 3: Student with 9 points (Total effort 9 <= 10)
This requires 3 teams.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One way to form minimal teams:
    - Team 1: Student with 2 points and student with 3 points (Total effort 5 <= 5)
    - Team 2: Two students with 2 points (Total effort 4 <= 5)
    - Team 3: Student with 4 points (Total effort 4 <= 5)
This requires 3 teams.

## Input Format

- The first line contains two integers n and x: the number of students and the maximum effort points per team.
- The second line contains n integers p_1, p_2, ..., p_n: the effort points of each student.

## Output Format

- Return a single integer: the minimum number of teams required.

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