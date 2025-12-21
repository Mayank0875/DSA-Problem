## Title
School Project Groups

## Slug
school-project-groups

## Difficulty
Hard

## Description
A teacher divides students into project teams. Each team picks a topic leader based on the most popular favorite subject ID among the team members.

Mrs. Krabappel has a collection of $n$ students, where each student is represented by an integer ID.

To organize the science fair, Mrs. Krabappel must partition these students into several non-empty teams. Every student from the original collection must belong to exactly one team. From each team, a "topic leader" is extracted. The topic leader is defined as the **mode** (most frequent element) of the students in that team. If a team has multiple students tied for the most frequent appearance, any one of them can be chosen as the topic leader.

Mrs. Krabappel collects all the extracted topic leaders to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> topic leader is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> topic leaders 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> topic leaders 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> topic leaders 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of students.
- The second line contains $n$ space-separated integers representing the student IDs.

## Output Format
- Return a single integer representing the number of different multisets of topic leaders possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
