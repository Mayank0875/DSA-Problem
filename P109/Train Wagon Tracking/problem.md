## Title
Train Wagon Tracking

## Slug
train-wagon-tracking

## Difficulty
Easy

## Description
A rail yard tracks wagons forming a train. Duplicate wagon IDs suggest a data entry error in the manifest.

Your task is to determine if any wagon ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The wagon ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All wagon IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of wagons.
- The second line contains n space-separated integers, representing the wagon IDs.

## Output Format
- Return `Yes` if any wagon ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
