## Title
Music Playlist Flow

## Slug
music-playlist-flow

## Difficulty
Medium

## Description
A DJ mixes tracks. Each track has an intro BPM and an outro BPM.

The crate contains list of tracks, each defined by a intro BPM and an outro BPM, represented as a pair `[intro, outro]`.

For a smooth 'ramp up' mix, the outro BPM of the current track must be strictly less than the intro BPM of the next track. Specifically, to transition from track `[a, b]` to a subsequent track `[c, d]`, the outro of the first track must be **strictly less than** the intro of the second track (i.e., `b < c`).

You can select tracks in any order you like to form a valid setlist. Your goal is to determine the maximum number of tracks that can be included in a single setlist.

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
The tracks can be reordered to form the setlist `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available tracks.
- The next `n` lines each contain two integers, representing the `intro` and `outro` of an track.

## Output Format
- Return a single integer representing the maximum length of the setlist.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ intro < outro ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
