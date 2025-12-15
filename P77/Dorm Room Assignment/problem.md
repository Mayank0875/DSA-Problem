## Title
Dorm Room Assignment

## Slug
dorm-room-assignment

## Difficulty
Medium

## Description
A university has `n` students applying for `m` available dorm rooms.

However, not every student is compatible with every room based on budget and preference.
You are given a list of `k` compatible pairs, where a specific student can work with a specific room.

Your task is to determine the maximum number of occupied rooms that can be formed simultaneously. Each student and each room can be assigned to at most one assignment.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 students and 2 rooms.
Possible valid matching could be:
- student 1 with room 2
- student 2 with room 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only student 1 and room 1 are compatible. The maximum number of operational occupied rooms is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of students, rooms, and compatible pairs.
- The students are numbered `1` to `n` and the rooms are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that student `a` and room `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
