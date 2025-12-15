## Title
Wedding Seating Plan

## Slug
wedding-seating-plan

## Difficulty
Medium

## Description
A planner seats `n` guests at `m` specific seats at the head table.

However, not every guest is compatible with every seat based on relationship status.
You are given a list of `k` compatible pairs, where a specific guest can work with a specific seat.

Your task is to determine the maximum number of seatings that can be formed simultaneously. Each guest and each seat can be assigned to at most one seating.

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
There are 3 guests and 2 seats.
Possible valid matching could be:
- guest 1 with seat 2
- guest 2 with seat 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only guest 1 and seat 1 are compatible. The maximum number of operational seatings is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of guests, seats, and compatible pairs.
- The guests are numbered `1` to `n` and the seats are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that guest `a` and seat `b` are compatible.

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
