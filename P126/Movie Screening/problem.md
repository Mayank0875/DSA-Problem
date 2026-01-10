## Title
Movie Screening

## Slug
movie-screening

## Difficulty
Easy

## Description
A cinema tracks movie showings across different screens.

The showtime list records the start time and end time of every movie in two integer arrays, `startTime` and `endTime`. The $i$-th movie starts at `startTime[i]` and ends at `endTime[i]`, inclusive.

The projectionist wants to know how many movies were playing during a specific prime time `[queryStart, queryEnd]`. A movie is considered playing if their screening overlaps with the prime time at any point (even for a single moment).

Your task is to return the total number of movies who were playing during the given prime time.

## Examples

### 1

#### Input
3
1 2 3
3 2 7
2 4

#### Output
3

#### Explanation
The prime time is `[2, 4]`.
- Movie 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Movie 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Movie 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 movies were playing.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The movie was playing at time `[4, 4]`. The prime time is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of movies.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of movies playing during the prime time.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 10^9
- 1 ≤ queryStart ≤ queryEnd ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, interval, linear-scan

## Company
amazon
