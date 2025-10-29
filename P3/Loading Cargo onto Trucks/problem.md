## Title

Loading Cargo onto Trucks

## Slug

loading-cargo-trucks

## Difficulty

Easy

## Description

A logistics company needs to transport cargo containers using trucks. Each truck can carry a maximum of two containers. However, the combined weight of containers on a truck must not exceed a limit `x`. You have `n` containers with known weights. Determine the minimum number of trucks required to transport all containers, ensuring the weight limit per truck is respected.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One way to load the trucks minimally:
    - Truck 1: Container weighing 2 and container weighing 7 (Total weight 9 <= 10)
    - Truck 2: Container weighing 3 (Total weight 3 <= 10)
    - Truck 3: Container weighing 9 (Total weight 9 <= 10)
This requires 3 trucks.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One way to load the trucks minimally:
    - Truck 1: Container weighing 2 and container weighing 3 (Total weight 5 <= 5)
    - Truck 2: Two containers weighing 2 (Total weight 4 <= 5)
    - Truck 3: Container weighing 4 (Total weight 4 <= 5)
This requires 3 trucks.

## Input Format

- The first line contains two integers n and x: the number of containers and the maximum allowed weight per truck.
- The second line contains n integers p_1, p_2, ..., p_n: the weight of each container.

## Output Format

- Return a single integer: the minimum number of trucks required.

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