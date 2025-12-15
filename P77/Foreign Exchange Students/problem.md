## Title
Foreign Exchange Students

## Slug
foreign-exchange-students

## Difficulty
Medium

## Description
The program matches `n` students with `m` host families.

However, not every student is compatible with every family based on language skills.
You are given a list of `k` compatible pairs, where a specific student can work with a specific family.

Your task is to determine the maximum number of placements that can be formed simultaneously. Each student and each family can be assigned to at most one placement.

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
There are 3 students and 2 families.
Possible valid matching could be:
- student 1 with family 2
- student 2 with family 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only student 1 and family 1 are compatible. The maximum number of operational placements is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of students, families, and compatible pairs.
- The students are numbered `1` to `n` and the families are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that student `a` and family `b` are compatible.

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
