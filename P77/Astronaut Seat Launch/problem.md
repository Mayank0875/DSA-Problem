## Title
Astronaut Seat Launch

## Slug
astronaut-seat-launch

## Difficulty
Medium

## Description
Mission control assigns `n` astronauts to `m` seats on the shuttle.

However, not every astronaut is compatible with every seat due to suit interface type.
You are given a list of `k` compatible pairs, where a specific astronaut can work with a specific seat.

Your task is to determine the maximum number of assignments that can be formed simultaneously. Each astronaut and each seat can be assigned to at most one assignment.

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
There are 3 astronauts and 2 seats.
Possible valid matching could be:
- astronaut 1 with seat 2
- astronaut 2 with seat 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only astronaut 1 and seat 1 are compatible. The maximum number of operational assignments is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of astronauts, seats, and compatible pairs.
- The astronauts are numbered `1` to `n` and the seats are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that astronaut `a` and seat `b` are compatible.

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
