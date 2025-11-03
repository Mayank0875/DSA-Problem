## Title

Shifted Historical Timeline

## Slug

shifted-historical-timeline

## Difficulty

Medium

## Description

A historian is examining a list of event dates (as unique integers) from an ancient text. The list was originally sorted by year, but the text is a fragment that starts from an unknown event, "rotating" the timeline (e.g., [1066, 1215, 1492] becomes [1492, 1066, 1215]). To understand the period, the historian needs to find the earliest event. Find the minimum date in the list in O(log n) time.

## Examples

### 1

#### Input

7
[4, 5, 6, 7, 0, 1, 2]

#### Output

0

#### Explanation

The smallest value in this rotated sequence is 0.

### 2

#### Input

6
[4, 5, 6, 7, 1, 2]

#### Output

1

#### Explanation

The smallest value in this rotated sequence is 1.

## Input Format

- The first line contains an integer n, the number of items.
- The second line contains n space-separated integers representing the item numbers after rotation. All numbers are unique.

## Output Format

- Return a single integer representing the minimum item number found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ gem_number ≤ 10^9
- The array is guaranteed to be a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array