## Title

The Corrupted Timeline

## Slug

the-corrupted-timeline

## Difficulty

Medium

## Description

A historian has discovered an scroll containing a list of historical events, represented by their years. A valid timeline must be chronological, meaning the years should appear in non-decreasing order.

However, a clumsy scribe seems to have inserted a chunk of incorrect years into the middle of the scroll, corrupting the timeline. To fix this, you must remove a single contiguous sequence of years (a subarray) so that the remaining years form a sorted, non-decreasing sequence.

Your goal is to minimize the loss of history. Determine the length of the shortest contiguous subarray that needs to be removed to restore the chronological order of the remaining events.

## Examples

### 1

#### Input

8 
1 2 3 10 4 2 3 5

#### Output

3

#### Explanation

The shortest subarray to remove is `[10, 4, 2]`. The remaining timeline is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.
    
### 2

#### Input

5 
5 4 3 2 1

#### Output

4

#### Explanation

Since the timeline is strictly decreasing, we can only keep one year. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]`).
  

## Input Format  

- The first line contains an integer `n`, the number of events.
- The second line contains `n` space-separated integers representing the `years` array.

## Output Format  

- Return a single integer representing the length of the shortest subarray to remove.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ year[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, two-pointers

## Company
flipkart