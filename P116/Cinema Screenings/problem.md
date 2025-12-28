## Title
Cinema Screenings

## Slug
cinema-screenings

## Difficulty
Medium

## Description
A movie theater plans screenings for a single screen. Each movie has a start and end time.

The list of list of movies, each defined by a start and an end, represented as a pair `[s, e]`.

Cleaning is required. The end time of a movie must be strictly less than the start of the next. Specifically, to transition from movie `[a, b]` to a subsequent movie `[c, d]`, the e of the first movie must be **strictly less than** the s of the second movie (i.e., `b < c`).

You can select movies in any order you like to form a valid showtimes. Your goal is to determine the maximum number of movies that can be included in a single showtimes.

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
The longest showtimes is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The movies can be reordered to form the showtimes `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available movies.
- The next `n` lines each contain two integers, representing the `s` and `e` of an movie.

## Output Format
- Return a single integer representing the maximum length of the showtimes.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ s < e ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
