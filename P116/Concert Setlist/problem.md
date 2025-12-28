## Title
Concert Setlist

## Slug
concert-setlist

## Difficulty
Medium

## Description
A band plans songs. Each song has a start minute and end minute in the show.

Song list: list of songs, each defined by a start and an end, represented as a pair `[s, e]`.

Songs cannot overlap. One must end strictly before the next starts. Specifically, to transition from song `[a, b]` to a subsequent song `[c, d]`, the e of the first song must be **strictly less than** the s of the second song (i.e., `b < c`).

You can select songs in any order you like to form a valid setlist. Your goal is to determine the maximum number of songs that can be included in a single setlist.

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
The longest setlist is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The songs can be reordered to form the setlist `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available songs.
- The next `n` lines each contain two integers, representing the `s` and `e` of an song.

## Output Format
- Return a single integer representing the maximum length of the setlist.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ s < e ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
