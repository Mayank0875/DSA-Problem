## Title
Shipping Containers

## Slug
shipping-containers

## Difficulty
Easy

## Description
A port crane scans container IDs. Duplicate IDs in the loading manifest could lead to lost cargo.

Your task is to determine if any container ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The container ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All container IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of containers.
- The second line contains n space-separated integers, representing the container IDs.

## Output Format
- Return `Yes` if any container ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
