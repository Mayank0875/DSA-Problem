## Title
Tutor Subject Match

## Slug
tutor-subject-match

## Difficulty
Medium

## Description
A tutoring center has `n` tutors and `m` subjects that need teaching slots.

However, not every tutor is compatible with every subject based on knowledge area.
You are given a list of `k` compatible pairs, where a specific tutor can work with a specific subject.

Your task is to determine the maximum number of classes that can be formed simultaneously. Each tutor and each subject can be assigned to at most one class.

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
There are 3 tutors and 2 subjects.
Possible valid matching could be:
- tutor 1 with subject 2
- tutor 2 with subject 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only tutor 1 and subject 1 are compatible. The maximum number of operational classes is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of tutors, subjects, and compatible pairs.
- The tutors are numbered `1` to `n` and the subjects are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that tutor `a` and subject `b` are compatible.

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
