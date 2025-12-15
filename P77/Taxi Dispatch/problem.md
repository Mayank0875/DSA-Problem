## Title
Taxi Dispatch

## Slug
taxi-dispatch

## Difficulty
Medium

## Description
There are `n` taxis and `m` passengers waiting in a zone. The dispatch system matches them.

However, not every taxi is compatible with every passenger based on proximity and destination.
You are given a list of `k` compatible pairs, where a specific taxi can work with a specific passenger.

Your task is to determine the maximum number of rides that can be formed simultaneously. Each taxi and each passenger can be assigned to at most one ride.

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
There are 3 taxis and 2 passengers.
Possible valid matching could be:
- taxi 1 with passenger 2
- taxi 2 with passenger 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only taxi 1 and passenger 1 are compatible. The maximum number of operational rides is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of taxis, passengers, and compatible pairs.
- The taxis are numbered `1` to `n` and the passengers are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that taxi `a` and passenger `b` are compatible.

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
