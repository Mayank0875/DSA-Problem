## Title
Mentor-Mentee Pairing

## Slug
mentor-mentee-pairing

## Difficulty
Medium

## Description
An organization has `n` mentors and `m` mentees. They want to form guidance pairs.

However, not every mentor is compatible with every mentee based on career goals.
You are given a list of `k` compatible pairs, where a specific mentor can work with a specific mentee.

Your task is to determine the maximum number of mentorships that can be formed simultaneously. Each mentor and each mentee can be assigned to at most one mentorship.

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
There are 3 mentors and 2 mentees.
Possible valid matching could be:
- mentor 1 with mentee 2
- mentor 2 with mentee 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only mentor 1 and mentee 1 are compatible. The maximum number of operational mentorships is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of mentors, mentees, and compatible pairs.
- The mentors are numbered `1` to `n` and the mentees are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that mentor `a` and mentee `b` are compatible.

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
