## Title

Bob's Unique Broadcasting Sequence

## Slug

bobs-unique-broadcasting-sequence

## Difficulty

Medium

## Description

Bob is a radio DJ who prides himself on variety. He has a playlist of $n$ songs, where each song is identified by a unique integer ID. The sequence of songs is currently arranged in a specific order.

Bob wants to analyze his playlist to find "perfect broadcasts." A perfect broadcast is defined as a contiguous sequence of songs from the playlist where every song is unique (no song is repeated within that sequence).

Bob wants to know how many such perfect broadcasts exist within his current playlist. Your task is to count the total number of contiguous subarrays where all elements are distinct.

## Examples

### 1

#### Input

4 
1 2 1 3

#### Output

8

#### Explanation

The distinct subarrays are: `[1]`, `[2]`, `[1]`, `[3]`, `[1,2]`, `[1,3]`, `[2,1]`, and `[2,1,3]`.
Subarray `[1,2,1]` is not counted because `1` repeats.
    
### 2

#### Input

5 
1 2 3 4 5

#### Output

15

#### Explanation

All elements are distinct. Every possible contiguous subarray is valid. The count is $5(6)/2 = 15$.

## Input Format  

- The first line contains an integer $n$, the number of songs in the playlist.
- The second line contains $n$ space-separated integers, representing the song IDs.

## Output Format  

- Return a single integer representing the number of subarrays with distinct elements.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, two-pointers, sliding-window

## Company
google