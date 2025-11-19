## Title
Nearest Lower Pressure Reading

## Slug
nearest-lower-pressure-reading

## Difficulty
Easy

## Description
You are an engineer monitoring the pressure inside a pipeline, measured at regular intervals. To detect pressure build-ups, you need to find the pressure value of the nearest previous interval that was strictly lower than the current reading. This helps in assessing the rate of pressure increase relative to the immediate past. For each pressure reading, you must find the value of the most recent preceding reading that was strictly smaller. If all previous readings were higher or equal, or if it is the start of the log, you should report a standard indicator. Your task is to analyze the pipeline pressure logs.

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
