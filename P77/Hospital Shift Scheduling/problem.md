## Title
Hospital Shift Scheduling

## Slug
hospital-shift-scheduling

## Difficulty
Medium

## Description
A hospital needs to assign `n` nurses to `m` available night shifts. A successful assignment ensures a shift is covered.

However, not every nurse is compatible with every shift due to certification requirements.
You are given a list of `k` compatible pairs, where a specific nurse can work with a specific shift.

Your task is to determine the maximum number of covered shifts that can be formed simultaneously. Each nurse and each shift can be assigned to at most one assignment.

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
There are 3 nurses and 2 shifts.
Possible valid matching could be:
- nurse 1 with shift 2
- nurse 2 with shift 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only nurse 1 and shift 1 are compatible. The maximum number of operational covered shifts is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of nurses, shifts, and compatible pairs.
- The nurses are numbered `1` to `n` and the shifts are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that nurse `a` and shift `b` are compatible.

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
