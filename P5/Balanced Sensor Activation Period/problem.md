## Title

Balanced Sensor Activation Period

## Slug

balanced-sensor-activation-period

## Difficulty

Easy

## Description

A system uses two types of sensors, type '0' and type '1'. A log records which sensor type was activated at N consecutive time points. Find the longest continuous period in the log where the number of activations of type '0' sensors equals the number of activations of type '1' sensors. This indicates a balanced sensor activity phase. Determine the length of the longest such balanced period.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The period [0, 1] (Type 0, Type 1) is the longest balanced activation period.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] and [1, 0] are the longest balanced activation periods.

## Input Format

- The first line contains a single integer N, the number of time points logged.
- The second line contains N space-separated integers, representing the sensor type activated (0 or 1).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced activation period.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sensors, prefix sum, hashmap