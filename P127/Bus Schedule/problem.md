## Title
Bus Schedule

## Slug
bus-schedule

## Difficulty
Medium

## Description
A commuter waits for buses. 1 is Arrival, 0 is No-Show. A taxi service can replace k no-show buses.

You track bus arrivals represented by an array `nums` consisting of 1s (arrivals) and 0s (no-shows), and an integer `k`. You are allowed to replace at most `k` no-showss from the sequence.

Your task is to find the length of the longest contiguous sequence of arrivalss after performing the replacements. If the sequence contains no arrivalss even after optimal replacements, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After replacing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of arrivalss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can replace the no-shows at index 4 and the no-shows at index 7. The resulting segments of arrivalss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for arrivals, 0 for no-shows).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of arrivalss.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ nums[i] ≤ 1
- 0 ≤ k ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array

## Company
facebook
