## Title

Logic Paradox: Nearest Stronger Statement

## Slug

logic-paradox-nearest-stronger-statement

## Difficulty

Easy

## Description

Imagine a sequence of logical statements, each assigned a numeric strength representing how paradoxical it is. As you examine each statement from left to right, you look back (to earlier statements) and want to know the strength of the nearest statement that is strictly stronger (more paradoxical) than the one you are currently considering. If all previous statements are weaker or of equal strength, or if it is the first statement, there is no such stronger statement to the left. Your goal is to determine this stronger statement's strength for each position in the sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Statement 0 (30): No previous statement. Output -1.
Statement 1 (60): Statement 0 (30) is weaker. Output -1.
Statement 2 (90): Statements 0 (30), 1 (60) are weaker. Output -1.
Statement 3 (50): Statement 2 (90) is the nearest stronger. Output 90.
Statement 4 (80): Statement 2 (90) is the nearest stronger. Output 90.
Statement 5 (40): Statement 4 (80) is the nearest stronger. Output 80.
Statement 6 (70): Statement 4 (80) is the nearest stronger. Output 80.
Statement 7 (50): Statement 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All statements have equal strength, so no strictly stronger previous statement exists.

## Input Format

The first line contains a single integer n, the number of statements.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the strength of each statement.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest statement j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array