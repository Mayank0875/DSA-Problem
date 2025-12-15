## Title
Cruise Ship Cabins

## Slug
cruise-ship-cabins

## Difficulty
Medium

## Description
A cruise line books `n` guests into `m` cabins.

However, not every guest is compatible with every cabin based on ticket class.
You are given a list of `k` compatible pairs, where a specific guest can work with a specific cabin.

Your task is to determine the maximum number of bookings that can be formed simultaneously. Each guest and each cabin can be assigned to at most one booking.

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
There are 3 guests and 2 cabins.
Possible valid matching could be:
- guest 1 with cabin 2
- guest 2 with cabin 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only guest 1 and cabin 1 are compatible. The maximum number of operational bookings is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of guests, cabins, and compatible pairs.
- The guests are numbered `1` to `n` and the cabins are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that guest `a` and cabin `b` are compatible.

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
