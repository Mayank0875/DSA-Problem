## Title
Taxi Rides

## Slug
taxi-rides

## Difficulty
Medium

## Description
A taxi driver selects rides. Each ride has a pickup mile marker and drop-off mile marker along a highway.

Available rides are list of rides, each defined by a pickup and an dropoff, represented as a pair `[pu, do]`.

The driver only drives forward. The dropoff of one ride must be strictly less than the pickup of the next. Specifically, to transition from ride `[a, b]` to a subsequent ride `[c, d]`, the do of the first ride must be **strictly less than** the pu of the second ride (i.e., `b < c`).

You can select rides in any order you like to form a valid trip. Your goal is to determine the maximum number of rides that can be included in a single trip.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest trip is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The rides can be reordered to form the trip `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available rides.
- The next `n` lines each contain two integers, representing the `pu` and `do` of an ride.

## Output Format
- Return a single integer representing the maximum length of the trip.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ pu < do ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
