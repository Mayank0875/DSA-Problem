## Title
The Longest Common Signal

## Slug
the-longest-common-signal

## Difficulty
Medium

## Description
Space researchers are analyzing radio transmissions received from two distant stars, Alpha and Beta. These transmissions are recorded as arrays of integer intensities. The researchers believe that a specific cosmic event occurred in the past, influencing both stars simultaneously. To confirm this theory, they need to find evidence of a shared pattern in the data.

Your task is to identify the longest continuous sequence of signal intensities that appears in both recordings. The sequence must be identical in both arrays and must not contain any gaps. You need to determine the length of this maximum matching subarray to help the researchers establish a connection between the two stars.

## Examples

### 1

#### Input
5
1 2 3 2 1
5
3 2 1 4 7

#### Output
3

#### Explanation
The longest common continuous signal is `[3, 2, 1]`, which has a length of 3.

### 2

#### Input
5
0 0 0 0 0
5
0 0 0 0 0

#### Output
5

#### Explanation
Both signals are identical and consist entirely of zeros. The longest common subarray is the entire signal itself, so the length is 5.

## Input Format
- The first line contains an integer `n`, the size of the first signal array.
- The second line contains `n` integers representing the first signal (`nums1`).
- The third line contains an integer `m`, the size of the second signal array.
- The fourth line contains `m` integers representing the second signal (`nums2`).

## Output Format
Return a single integer representing the maximum length of a subarray that appears in both arrays.

## Constraints
- 1 ≤ n, m ≤ 1000
- 1 ≤ nums1[i], nums2[i] ≤ 100

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, sliding-window