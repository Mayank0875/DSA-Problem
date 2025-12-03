## Title
Social Media Circles

## Slug
social-media-circles

## Difficulty
Hard

## Description
A new social app has n users. Friendships connect some users into social circles. The algorithm boosts visibility for circles whose member count is a 'Viral Number'—containing only digits 4 and 7.

A marketer wants to create such a circle by introducing users. Merging k existing circles requires k - 1 new introductions.

Your task is to determine the minimum number of extra introductions the marketer needs to build to create at least one circle whose size is a Viral Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect user 4 with user 3. We can also connect 4 with 1 or 2. This creates a circle of size 4 (a Viral Number).

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
There is no way to connect the users to form a circle with a size equal to a Viral Number.

## Input Format
- The first line contains two integers n and m: the number of users and the number of existing introductions.
- The next m lines each contain two integers u and v, representing a friendship between user u and user v. Note that u may be equal to v, and there may be multiple introductions connecting the same pair of users.

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
