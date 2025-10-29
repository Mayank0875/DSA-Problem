## Title

Unique Songs Played on Radio

## Slug

unique-songs-played-radio

## Difficulty

Easy

## Description

A radio station DJ kept a log of every song played during their shift. Each song is identified by a unique numerical ID. Since popular songs might be played multiple times, the log contains duplicate entries. The DJ wants to report the total number of different songs played, not the total number of plays. Given the list of song IDs from the log, determine the count of unique songs that were aired.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The song IDs logged are 2, 3, 2, 2, 3. The unique song IDs are 2 and 3. There were 2 distinct songs played.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique song IDs are 10, 5, and 2. There were 3 distinct songs played.

## Input Format

- The first line contains an integer n: the total number of songs logged.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the song identification codes.

## Output Format

- Return a single integer: the count of distinct song IDs.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, music