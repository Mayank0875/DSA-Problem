## Title

Loading Items onto Delivery Drones

## Slug

loading-items-delivery-drones

## Difficulty

Easy

## Description

A company uses delivery drones, each capable of carrying one or two packages per trip. However, the total weight of the package(s) on a drone must not exceed its capacity `x`. You have `n` packages with specified weights waiting for delivery. Calculate the minimum number of drone trips needed to deliver all packages, respecting the weight capacity of each drone trip.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One way to minimize trips:
    - Trip 1: Drone carries package weighing 2 and package weighing 7 (Total weight 9 <= 10)
    - Trip 2: Drone carries package weighing 3 (Total weight 3 <= 10)
    - Trip 3: Drone carries package weighing 9 (Total weight 9 <= 10)
This requires 3 trips.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One way to minimize trips:
    - Trip 1: Drone carries package weighing 2 and package weighing 3 (Total weight 5 <= 5)
    - Trip 2: Drone carries two packages weighing 2 (Total weight 4 <= 5)
    - Trip 3: Drone carries package weighing 4 (Total weight 4 <= 5)
This requires 3 trips.

## Input Format

- The first line contains two integers n and x: the number of packages and the maximum weight capacity per drone trip.
- The second line contains n integers p_1, p_2, ..., p_n: the weight of each package.

## Output Format

- Return a single integer: the minimum number of drone trips required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers