## Title
Musician Gig Booking

## Slug
musician-gig-booking

## Difficulty
Medium

## Description
An agency books `n` musicians for `m` venues on Friday night.

However, not every musician is compatible with every venue based on genre fit.
You are given a list of `k` compatible pairs, where a specific musician can work with a specific venue.

Your task is to determine the maximum number of gigs that can be formed simultaneously. Each musician and each venue can be assigned to at most one gig.

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
There are 3 musicians and 2 venues.
Possible valid matching could be:
- musician 1 with venue 2
- musician 2 with venue 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only musician 1 and venue 1 are compatible. The maximum number of operational gigs is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of musicians, venues, and compatible pairs.
- The musicians are numbered `1` to `n` and the venues are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that musician `a` and venue `b` are compatible.

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
