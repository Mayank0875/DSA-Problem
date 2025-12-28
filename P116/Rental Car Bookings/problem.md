## Title
Rental Car Bookings

## Slug
rental-car-bookings

## Difficulty
Medium

## Description
A single car is available for rent. Requests come in with pickup and drop-off dates.

Requests list list of bookings, each defined by a pickup day and an dropoff day, represented as a pair `[pickup, dropoff]`.

The car needs cleaning between rentals. The dropoff day of one rental must be strictly before the pickup day of the next. Specifically, to transition from booking `[a, b]` to a subsequent booking `[c, d]`, the dropoff of the first booking must be **strictly less than** the pickup of the second booking (i.e., `b < c`).

You can select bookings in any order you like to form a valid schedule. Your goal is to determine the maximum number of bookings that can be included in a single schedule.

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
The longest schedule is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The bookings can be reordered to form the schedule `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available bookings.
- The next `n` lines each contain two integers, representing the `pickup` and `dropoff` of an booking.

## Output Format
- Return a single integer representing the maximum length of the schedule.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ pickup < dropoff ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
