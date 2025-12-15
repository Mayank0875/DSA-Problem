## Title
Police Patrol Beats

## Slug
police-patrol-beats

## Difficulty
Medium

## Description
A precinct assigns `n` officers to `m` patrol beats.

However, not every officer is compatible with every beat based on district familiarity.
You are given a list of `k` compatible pairs, where a specific officer can work with a specific beat.

Your task is to determine the maximum number of assignments that can be formed simultaneously. Each officer and each beat can be assigned to at most one assignment.

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
There are 3 officers and 2 beats.
Possible valid matching could be:
- officer 1 with beat 2
- officer 2 with beat 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only officer 1 and beat 1 are compatible. The maximum number of operational assignments is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of officers, beats, and compatible pairs.
- The officers are numbered `1` to `n` and the beats are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that officer `a` and beat `b` are compatible.

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
