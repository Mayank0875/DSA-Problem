## Title
Last Smaller Crowd Size

## Slug
last-smaller-crowd-size

## Difficulty
Easy

## Description
You are an event organizer analyzing attendance numbers for a series of weekly concerts. You have a list of crowd sizes for each week. To understand popularity trends, you want to identify the attendance number of the nearest previous week that was strictly smaller than the current week's attendance. This helps in gauging recent growth in audience size. For each week's crowd size, your goal is to find the value of the most recent preceding week where the attendance was strictly lower. If no such week exists (e.g., attendance has been dropping or constant), you must report a standard indicator. Your task is to calculate this metric for every week.

## Examples

### 1

#### Input
8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output
[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation
Index 0 (100): No previous value, output -1.
Index 1 (80): 100 is not lower, output -1.
Index 2 (60): 100, 80 are not lower, output -1.
Index 3 (70): 60 is the nearest lower value, output 60.
Index 4 (60): No strictly lower previous value, output -1.
Index 5 (75): 60 at index 4 is nearest lower, output 60.
Index 6 (85): 75 at index 5 is nearest lower, output 75.
Index 7 (110): 85 at index 6 is nearest lower, output 85.

### 2

#### Input
5
50 50 50 50 50

#### Output
[-1, -1, -1, -1, -1]

#### Explanation
All values are equal, so no strictly lower previous value exists for any element.

## Input Format
The first line contains a single integer n, the number of elements.
The second line contains n space-separated integers representing the data sequence.

## Output Format
Return array of integers. The i-th integer should be the value of the nearest element j < i such that val_j < val_i. If no such element exists, return -1.

## Constraints
1 ≤ n ≤ 10^5
1 ≤ val_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, array
