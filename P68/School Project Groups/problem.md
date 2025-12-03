## Title
School Project Groups

## Slug
school-project-groups

## Difficulty
Hard

## Description
n students are in a class. Some are friends, forming groups. The teacher assigns special projects to groups whose size is a 'Grade A Number' (digits 4 and 7).

You can introduce students to merge groups. Merging k groups requires k - 1 introductions.

Your task is to determine the minimum number of extra introductions the teacher needs to build to create at least one group whose size is a Grade A Number. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect student 4 with student 3. We can also connect 4 with 1 or 2. This creates a group of size 4 (a Grade A Number).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the students to form a group with a size equal to a Grade A Number.

## Input Format
- The first line contains two integers n and m: the number of students and the number of existing introductions.
- The next m lines each contain two integers u and v, representing a friendship between student u and student v. Note that u may be equal to v, and there may be multiple introductions connecting the same pair of students.

## Output Format
- Return a single integer: the minimum number of introductions to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
