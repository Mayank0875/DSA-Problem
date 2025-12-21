## Title
Music Playlist

## Slug
music-playlist

## Difficulty
Hard

## Description
Songs are grouped into mini-mixes. The genre of the mix is defined by the most frequent song genre ID within it.

DJ Sona has a collection of $n$ songs, where each song is represented by an integer ID.

To curate the festival set, DJ Sona must partition these songs into several non-empty mixes. Every song from the original collection must belong to exactly one mix. From each mix, a "dominant genre" is extracted. The dominant genre is defined as the **mode** (most frequent element) of the songs in that mix. If a mix has multiple songs tied for the most frequent appearance, any one of them can be chosen as the dominant genre.

DJ Sona collects all the extracted dominant genres to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> dominant genre is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> dominant genres 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> dominant genres 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> dominant genres 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of songs.
- The second line contains $n$ space-separated integers representing the song IDs.

## Output Format
- Return a single integer representing the number of different multisets of dominant genres possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
