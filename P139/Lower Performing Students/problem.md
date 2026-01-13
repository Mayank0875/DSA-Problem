## Title
Lower Performing Students

## Slug
lower-performing-students

## Difficulty
Medium

## Description
A school analyzes test results.

You have a list of $n$ students. Each student has two main properties: **math score** and **science score**. You are given a 2D integer array `properties` where `properties[i] = [math score_i, science score_i]` represents the attributes of the $i$-th student.

A student is considered **lower performing** if there exists another student that has **both** strictly greater math score and strictly greater science score.

More formally, the $i$-th student is lower performing if there exists an index $j$ such that `math score_j > math score_i` and `science score_j > science score_i`.

Your task is to return the number of lower performing students.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No student has strictly greater math score and science score than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first student (2, 2) is lower performing because the second student (3, 3) has strictly greater math score and science score.

## Input Format
- The first line contains an integer $n$, the number of students.
- The next $n$ lines each contain two space-separated integers, representing the math score and science score of a student.

## Output Format
- Return a single integer representing the number of lower performing students.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ math score, science score ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
